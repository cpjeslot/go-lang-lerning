
# Go Conference Ticket Booking Application

This is a simple Go application to manage the ticket booking process for a conference. The application handles user inputs, validates them, and books tickets while tracking the remaining tickets. It also sends a simulated email confirmation asynchronously.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Features

- Book tickets for a conference.
- Validate user inputs (first name, last name, email, and ticket count).
- Display the list of attendees by first name.
- Asynchronous ticket confirmation using goroutines.
- Track remaining tickets and notify when the event is sold out.

## Prerequisites

- Go 1.24.1 installed on your machine.
- Basic understanding of Go programming.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/cpjeslot/go-lang-lerning.git
   ```

2. Navigate to the project directory:

   ```bash
   cd conference-booking-app
   ```

3. Run the application:

   ```bash
   go run main.go
   ```

## Usage

1. Upon running the program, you will be greeted with information about the conference, including the total number of tickets available.
2. The program will prompt you to enter your first name, last name, email address, and the number of tickets you wish to book.
3. The input will be validated, and if valid, your tickets will be booked, and a confirmation message will be displayed.
4. The system will asynchronously "send" the ticket to the provided email address after a 50-second delay.
5. The application will stop when all tickets are booked.

### Example Workflow

```
Welcome to Go Conference booking application
We have total of 50 tickets and 50 are still available.
Get your tickets here to attend

Enter your first name: John
Enter your last name: Doe
Enter your email address: john.doe@example.com
Enter number of tickets: 2
Thank you John Doe for booking 2 tickets. You will receive a confirmation email at john.doe@example.com
48 tickets remaining for Go Conference
Sending ticket: 2 tickets for John Doe to email address john.doe@example.com
```

## Contributing

If you wish to contribute to the project, feel free to fork the repository and submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a pull request

## Acknowledgments

This project was created as part of a Go programming tutorial by **Nana Janashia**. You can watch the full tutorial on YouTube [here](https://www.youtube.com/watch?v=yyUHQIec83I).

---

Developed by: Chetan Patel  
Email: chetan@jeslot.in
