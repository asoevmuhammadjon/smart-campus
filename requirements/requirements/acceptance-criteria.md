# Acceptance Criteria

This document defines the acceptance criteria for three core user stories (US-01, US-02, and US-05) using standard Given-When-Then format.

## AC for US-01: Browse Available Rooms
* **Scenario 1: Successful filtering of study rooms**
  * **Given** the student is on the room search dashboard,
  * **When** they filter by capacity (minimum 4 people) and equipment ("Whiteboard"),
  * **Then** the system displays a list of rooms matching all filter criteria.

* **Scenario 2: No rooms match criteria**
  * **Given** the student selects strict filters with zero availability,
  * **When** the search query is executed,
  * **Then** the system displays a clear message "No study rooms available for the selected filters and time slot."

---

## AC for US-02: Book a Study Room
* **Scenario 1: Successful booking creation**
  * **Given** an eligible student has selected an open time slot (e.g., 14:00 - 16:00) for Room A101,
  * **When** they click "Confirm Booking",
  * **Then** the reservation is saved in the database, a confirmation message is displayed, and the slot shows as booked.

* **Scenario 2: Exceeding daily time limit rule**
  * **Given** the student already has 3 hours of bookings for the current day,
  * **When** they attempt to book another room,
  * **Then** the system rejects the request and displays an error message regarding the 3-hour daily limit rule (BR1).

---

## AC for US-05: Digital Check-in via QR Code
* **Scenario 1: Successful check-in within window**
  * **Given** the student has an active booking starting at 14:00 and current time is 14:05,
  * **When** they scan the room's QR code using the web app,
  * **Then** the system marks the status as "Checked-In" and unlocks digital logs.

* **Scenario 2: Late check-in auto-cancellation**
  * **Given** the booking start time was 14:00 and current time is 14:16 (past the 15-minute window),
  * **When** the student attempts to check in,
  * **Then** the system rejects the check-in, marks the booking as "Auto-Cancelled" (BR3), and releases the room.
