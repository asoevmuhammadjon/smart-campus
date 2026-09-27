# User Stories - Smart Campus Study Room Booking

## Overview
This document contains 7 user stories derived from the Smart Campus study room booking scenario, complete with priorities, unique identifiers, and underlying assumptions.

---

## User Stories

### US-01: Browse Available Rooms
* **ID:** US-01
* **Priority:** High
* **As a** registered university student,
* **I want to** view a list of available study rooms with filters for capacity, date, time slot, and equipment (e.g., whiteboard, display screen),
* **So that** I can find a suitable room for my group study session.
* **Assumptions:** 
  * Room metadata (capacity, equipment) is pre-configured in the system by the facilities admin.
  * Real-time availability updates instantly upon selection.

### US-02: Book a Study Room
* **ID:** US-02
* **Priority:** High
* **As a** registered university student,
* **I want to** reserve an available study room for a specific time slot (up to 3 hours),
* **So that** I have a guaranteed quiet space for academic work.
* **Assumptions:**
  * The student has no overlapping active bookings for the same time slot.
  * Bookings can be made up to 7 days in advance.

### US-03: Cancel a Booking
* **ID:** US-03
* **Priority:** Medium
* **As a** registered university student,
* **I want to** cancel an existing study room reservation,
* **So that** the room becomes available for other students if my plans change.
* **Assumptions:**
  * Cancellation can be performed at any time before the booking start time without penalty.

### US-04: View Active and Past Bookings
* **ID:** US-04
* **Priority:** Medium
* **As a** registered university student,
* **I want to** view my personal history of active and past study room bookings,
* **So that** I can keep track of my scheduled study sessions.
* **Assumptions:**
  * Past bookings are archived automatically after 30 days.

### US-05: Digital Check-in via QR Code
* **ID:** US-05
* **Priority:** High
* **As a** registered university student,
* **I want to** check in to my booked room by scanning a QR code near the entrance within 15 minutes of the start time,
* **So that** the system verifies my attendance and prevents auto-cancellation.
* **Assumptions:**
  * Every study room has a unique physical QR code sticker placed at the entrance.

### US-06: Manage Room Maintenance and Availability (Admin)
* **ID:** US-06
* **Priority:** Medium
* **As a** Campus Facilities Administrator,
* **I want to** mark a study room as "Under Maintenance" or unavailable,
* **So that** students cannot book rooms that are undergoing repairs.
* **Assumptions:**
  * Existing bookings for a room marked under maintenance are automatically cancelled and notified to affected users.

### US-07: Generate Room Utilization Reports (Admin)
* **ID:** US-07
* **Priority:** Low
* **As a** Campus Facilities Administrator,
* **I want to** generate analytical reports on room utilization rates,
* **So that** administration can optimize space allocation across campus.
* **Assumptions:**
  * Reports can be filtered by date range and building location.
