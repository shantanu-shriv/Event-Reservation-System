# Multi-threaded Event Reservation System

## Overview

The Multi-threaded Event Reservation System is a concurrent application designed to handle event reservations using POSIX threads (pthreads). This system supports various operations such as booking tickets, canceling reservations, and checking seat availability across multiple events. It employs mutexes and condition variables to ensure thread safety and proper synchronization between threads.

## Features

- **Concurrent Reservation Handling**: Efficiently manages event reservations with the help of multiple worker threads, enabling simultaneous query processing.
- **Thread Synchronization**: Utilizes mutexes and condition variables to ensure data consistency and prevent race conditions during concurrent access.
- **Dynamic Query Processing**: Supports various types of queries including:
  - Ticket booking
  - Ticket cancellation
  - Seat availability checks
- **Simulation of Operation Time**: Incorporates random delays to simulate real-world processing times and system load, mimicking a real-time environment.

## Project Structure

- **event_reservation.c**: Contains the core logic of the reservation system, including:
  - Thread creation and management
  - Synchronization mechanisms using mutexes and condition variables
  - Query processing logic for booking, cancellation, and seat availability

## Getting Started

### Prerequisites

- **C Compiler**: A C compiler like `gcc` is required to compile the source code.
- **POSIX Threads Library**: Ensure the system has the pthreads library installed for threading support.

### Compilation

To compile the project, use the following command:

```bash
gcc event_reservation.c
./a.out
```

