# RailBandhu

This project is a mini railway reservation system based on Indian Railway Ticket Reservation System implemented using SQL. It allows users to book and cancel train tickets, manage seat availability, track revenue, and handle waitlists. The system simulates the core functionalities of a real-world railway ticketing platform, designed for learning and demonstration purposes.

Key Features:
1. Ticket Booking – Users can book tickets based on train, class, date, and number of passengers.
2. Ticket Cancellation – Booked tickets can be cancelled; the system automatically updates availability and waitlist accordingly.
3. Seat Availability Check – Users can check how many seats are available in a given class of a train on a specific date.
4. Waitlist Management – If seats are unavailable, bookings are placed on a waitlist and promoted automatically when cancellations occur.
5. Refund Management – Refunds are calculated based on cancellation timing and rules.
6. Revenue Tracking – Tracks revenue generated per train, per date, and overall.
7. Comprehensive Reporting – Includes queries for top earning trains, fully booked trains, most popular routes, and more.

Database Components
- Tables: Station, Train, Route, Class, Seat, Passenger, Ticket, Cancellation, Payment 
- Potential Queries:
- PNR status tracking for a given ticket.
- Train schedule lookup for a given train.
- Available seats query for a specific train, date and class.
- List all passengers traveling on a specific train on a given date.
- Retrieve all waitlisted passengers for a particular train.
- Find total amount that needs to be refunded for cancelling a train.
- Total revenue generated from ticket bookings over a specified period.
- Cancellation records with refund status.
- Find the busiest route based on passenger count.
- Generate an itemized bill for a ticket including all charges.
- Stored Procedures and Functions:
    - billing_desk()
    - cancel_ticket()
    - train_schedule()
    - available_seats ()
    - refund_for_cancelling_train()
    - total_convenience_fee_revenue()
    - waitlisted_passengers()
    - generate_itemized_bill()
- Triggers: Automatic handling for waitlist updates and ticket ID generation

Technologies Used:
- SQL (MySQL / PostgreSQL syntax)
- ER Modeling & Relational Schema Design
- Queries, Stored Procedures, Functions, and Triggers

Usage Instructions:
1. Import the SQL script files to create tables and insert initial data.
2. Load the stored procedures and functions into your database.
3. Execute SQL queries to book/cancel tickets.
4. Use sample test cases provided to validate functionality.
5. Ticket data is given before importing run trigger for Automatic Payment Schema insertion.
6. After loading data for Ticket Schema drop trigger for automatic Payment Schema insertion.

Project Files Included:
-CSV data files
-SQL file
-Project Documentation File
- README.txt – This file
