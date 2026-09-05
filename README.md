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

┌───────────────────────────────┐
│            USER               │
│        👤 Customer            │
└───────────────┬───────────────┘
                │
                ▼
╔══════════════════════════════════════════════════════════════╗
║                    FRONTEND / UI                            ║
║                                                              ║
║  ┌──────────────┐   ┌──────────────┐   ┌─────────────────┐  ║
║  │ Login /      │   │ Movie        │   │ Movie Details   │  ║
║  │ Registration │   │ Search       │   │ & Trailer       │  ║
║  └──────────────┘   └──────────────┘   └─────────────────┘  ║
║                                                              ║
║  ┌──────────────┐   ┌──────────────┐   ┌─────────────────┐  ║
║  │ Theatre &    │   │ Seat         │   │ Booking         │  ║
║  │ Show         │   │ Selection    │   │ Summary         │  ║
║  └──────────────┘   └──────────────┘   └─────────────────┘  ║
║                                                              ║
║  ┌──────────────┐   ┌──────────────┐   ┌─────────────────┐  ║
║  │ Payment      │   │ My Bookings  │   │ Digital Ticket  │  ║
║  │ Page         │   │ & Cancellation│  │ + QR Code       │  ║
║  └──────────────┘   └──────────────┘   └─────────────────┘  ║
╚═══════════════════════╤══════════════════════════════════════╝
                        │
                 HTTP / REST API
                        │
                        ▼
╔══════════════════════════════════════════════════════════════╗
║                     BACKEND / SERVER                        ║
║                                                              ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                  Authentication Module                 │  ║
║  │        Login • Registration • Password Reset           │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                    Movie Module                        │  ║
║  │     Browse • Search • Filter • Movie Details           │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │              Theatre & Show Module                     │  ║
║  │       City • Theatre • Date • Showtime • Seats          │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                   Booking Module                       │  ║
║  │   Seat Availability • Booking • Booking ID • Summary   │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                   Payment Module                       │  ║
║  │          Payment Processing • Success / Failure        │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                 Ticket Module                          │  ║
║  │       E-Ticket • QR Code • Email Confirmation           │  ║
║  └────────────────────────────────────────────────────────┘  ║
║                          │                                   ║
║  ┌────────────────────────────────────────────────────────┐  ║
║  │                  Admin Module                           │  ║
║  │ Movies • Theatres • Shows • Users • Bookings • Payments │  ║
║  └────────────────────────────────────────────────────────┘  ║
╚═══════════════════════╤══════════════════════════════════════╝
                        │
                    SQL / ORM
                        │
                        ▼
╔══════════════════════════════════════════════════════════════╗
║                       DATABASE                              ║
║                                                              ║
║  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌────────────┐  ║
║  │  Users   │  │  Movies  │  │ Theatres │  │   Shows    │  ║
║  └──────────┘  └──────────┘  └──────────┘  └────────────┘  ║
║                                                              ║
║  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌────────────┐  ║
║  │  Seats   │  │ Bookings │  │ Payments │  │  Tickets   │  ║
║  └──────────┘  └──────────┘  └──────────┘  └────────────┘  ║
║                                                              ║
║  ┌──────────┐                                               ║
║  │  Admins  │                                               ║
║  └──────────┘                                               ║
╚══════════════════════════════════════════════════════════════╝

                         BACKEND
                       ↙          ↘
                      ↙            ↘
             ┌──────────────┐   ┌────────────────┐
             │   PAYMENT    │   │ EMAIL SERVICE  │
             │   GATEWAY    │   │                │
             │              │   │ E-Ticket + QR  │
             └──────────────┘   └────────────────┘
