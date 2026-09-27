# Requirements Traceability Matrix

| Requirement ID | Requirement Type | Description / Name | Associated Use Cases | Test / AC Reference | Status |
|----------------|------------------|--------------------|----------------------|---------------------|--------|
| BR-01          | Business Rule    | Max 3 hours/day per student | US-02 | AC-US02-S2          | Verified |
| BR-02          | Business Rule    | Advance booking window (1h to 7d) | US-02 | AC-US02-S1          | Verified |
| BR-03          | Business Rule    | 15-minute QR check-in auto-release | US-05 | AC-US05-S2          | Verified |
| BR-04          | Business Rule    | Valid campus ID check required | US-02, US-05 | System Auth | Verified |
| US-01          | User Story       | Browse Available Rooms | UC1 | AC-US01-S1, S2      | Implemented |
| US-02          | User Story       | Book a Study Room | UC2 | AC-US02-S1, S2      | Implemented |
| US-03          | User Story       | Cancel a Booking | UC3 | Unit Test #3        | Implemented |
| US-04          | User Story       | View Active/Past Bookings | UC4 | Unit Test #4        | Implemented |
| US-05          | User Story       | Digital Check-in via QR | UC5 | AC-US05-S1, S2      | Implemented |
| US-06          | User Story       | Manage Room Maintenance | UC6 | Admin Test #1       | Implemented |
| US-07          | User Story       | Generate Utilization Reports | UC7 | Admin Test #2       | Implemented |
