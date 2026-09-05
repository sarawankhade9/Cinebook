# Cinebook
A full-featured online movie ticket booking system that allows users to browse and search movies, view movie details, select theatres and showtimes, choose seats, make online payments, and receive digital tickets with QR codes via email. The system also includes admin panel for managing movies, theatres, shows, seats, users, bookings, and payment
                         MOVIE TICKET BOOKING SYSTEM
                  ┌─────────────────────────────────────────┐
                  │                                         │
                  │        (User Registration / Login)      │
                  │                    │                    │
                  │                    ▼                    │
                  │             (Browse Movies)             │
                  │                    │                    │
                  │                    ▼                    │
                  │             (Select Movie)              │
                  │                    │                    │
                  │                    ▼                    │
                  │        (Select Theatre & Show)          │
                  │                    │                    │
                  │                    ▼                    │
                  │             (Select Seats)               │
                  │                    │                    │
                  │                    ▼                    │
                  │             (Book Ticket)               │
                  │                    │                    │
                  │                    ▼                    │
                  │                (Payment)                │
                  │                    │                    │
                  │                    ▼                    │
                  │          (Booking Confirmation)         │
                  │                    │                    │
                  │                    ▼                    │
                  │          (Send Ticket to Email)        │
                  │                                         │
                  └─────────────────────────────────────────┘
                         ▲                    ▲
                         │                    │
                       User            Payment Gateway
                                             
                                             ▲
                                             │
                                      Email Service







                                      features /updatation

                                                               ┌─────────────────────────────────────────────┐
                         │       MOVIE TICKET BOOKING SYSTEM            │
                         │                                             │
 USER                    │                                             │
  │                      │  ○ Register                                 │
  ├─────────────────────►│  ○ Login / Logout                           │
  │                      │  ○ Forgot Password                           │
  │                      │                                             │
  ├─────────────────────►│  ○ Browse Movies                            │
  │                      │  ○ Search Movies                            │
  │                      │  ○ Filter Movies                            │
  │                      │  ○ View Movie Details                       │
  │                      │                                             │
  ├─────────────────────►│  ○ Select City / Location                   │
  │                      │  ○ Select Theatre                            │
  │                      │  ○ Select Date & Showtime                    │
  │                      │  ○ Select Seats                              │
  │                      │                                             │
  ├─────────────────────►│  ○ Book Ticket                              │
  │                      │       │                                     │
  │                      │       │ <<include>>                         │
  │                      │       ▼                                     │
  │                      │  ○ Booking Summary                          │
  │                      │       │                                     │
  │                      │       │ <<include>>                         │
  │                      │       ▼                                     │
  │                      │  ○ Make Payment ◄──────── PAYMENT GATEWAY    │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Booking Confirmation                     │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Generate E-Ticket                        │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Generate QR Code                         │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Send Ticket by Email ─────► EMAIL SERVICE │
  │                      │                                             │
  ├─────────────────────►│  ○ My Bookings                             │
  │                      │       ├── ○ Upcoming Bookings               │
  │                      │       ├── ○ Previous Bookings                │
  │                      │       └── ○ View Ticket                      │
  │                      │                                             │
  ├─────────────────────►│  ○ Cancel Booking                           │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Request Refund                            │
  │                      │       │                                     │
  │                      │       ▼                                     │
  │                      │  ○ Check Refund Status                       │
  │                      │                                             │
                         └─────────────────────────────────────────────┘


 ADMIN
  │
  ├─────────────────────► ○ Admin Login
  ├─────────────────────► ○ Manage Movies
  │                         ├── Add Movie
  │                         ├── Update Movie
  │                         └── Delete Movie
  │
  ├─────────────────────► ○ Manage Theatres
  │
  ├─────────────────────► ○ Manage Shows
  │
  ├─────────────────────► ○ Manage Seats
  │
  ├─────────────────────► ○ Manage Users
  │
  ├─────────────────────► ○ View Bookings
  │
  └─────────────────────► ○ View Payments
