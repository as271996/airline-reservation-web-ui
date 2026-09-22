# Airline Reservation Web UI

A front-end airline reservation website prototype built using **HTML, CSS, and JavaScript**.

The project demonstrates a simple multi-page airline booking interface where users can browse flight information, access signup and login forms, and enter passenger details through a booking form.

The website includes:

- Home page with navigation to the main sections
- User signup form
- Login form
- Flight information page
- Airline booking form
- Client-side JavaScript form validation
- Shared CSS styling across the website

This project was developed to practice core front-end concepts including multi-page website structure, form design, navigation, styling, and browser-side input validation.

## Features

- Multi-page airline reservation website interface
- Home page with navigation across all major sections
- User signup form with client-side validation
- Login form with email and password validation
- Flight information page displaying:
  - flight number
  - origin
  - destination
  - departure time
- Booking form with:
  - origin selection
  - destination selection
  - one-way or round-trip choice
  - economy or business class selection
  - payment mode selection
  - terms and conditions confirmation
- Shared navigation menu across pages
- JavaScript-based form validation for required fields
- Email-format validation
- Password confirmation validation during signup
- Shared CSS styling for layout, navigation, and page presentation

## Website Structure and Navigation Flow

The project is organized as a small multi-page static website.

```text
Home
 │
 ├── Sign Up
 │
 ├── Log In
 │
 ├── Flights
 │
 └── Book Now
```

Each page includes navigation links to the other major sections of the website.

### Pages

#### Home — `air.html`

The landing page of the website.

It provides:

- the main navigation menu
- introductory airline content
- a direct link to the booking page

#### Sign Up — `air_signup.html`

Provides a user-registration form with fields such as:

- first name
- last name
- email address
- password and password confirmation
- gender
- country
- language preferences
- alternate email address
- agreement confirmation

JavaScript validation is performed before the form is submitted.

#### Log In — `air_login.html`

Provides a simple login interface with:

- email address
- password
- stay-signed-in option

The page performs client-side validation before submission.

#### Flights — `air_flights.html`

Displays static flight information in tabular form, including:

- flight number
- origin
- destination
- departure time

#### Book Now — `air_book.html`

Provides the airline booking interface where users can select:

- origin
- destination
- one-way or round-trip travel
- economy or business class
- payment mode
- acceptance of terms and conditions

The form uses JavaScript validation before submission.

### Navigation

The same navigation pattern is used across the main pages:

```text
Home | Sign Up | Log In | Flights | Book Now
```

This allows users to move directly between the different sections of the website without returning to the home page.

## Tech Stack

**Frontend:** HTML5, CSS3, JavaScript  
**Styling:** Custom CSS  
**Validation:** Vanilla JavaScript  
**Architecture:** Multi-page static website  

## Project Structure

```text
airline-reservation-web-ui/
├── air.html
├── air_book.html
├── air_css.css
├── air_flights.html
├── air_login.html
└── air_signup.html
```

### Main Files

`air.html`  
Main landing page and navigation entry point for the website.

`air_signup.html`  
Contains the user-registration interface and signup form validation.

`air_login.html`  
Contains the login interface and client-side credential-field validation.

`air_flights.html`  
Displays the available flight information in a table.

`air_book.html`  
Contains the airline booking form and booking-related input validation.

`air_css.css`  
Provides the shared styling used across the website, including navigation, forms, tables, and page layout.

## Form Validation and User Interaction

The project uses vanilla JavaScript to perform basic client-side validation before form submission.

### Signup Validation

The signup form validates:

- first name is not empty
- last name is not empty
- email address follows a basic email format
- password is provided
- password confirmation is provided
- password and confirmation values match
- gender is selected
- agreement checkbox is selected

```text
User fills signup form
        │
        ▼
JavaScript Validation
        │
        ├── Invalid Input ──► Alert Message
        │
        └── Valid Input ────► Form Submission
```

### Login Validation

The login page checks:

- email address format
- password is not empty
- the stay-signed-in checkbox is selected

If validation fails, the user receives a browser alert and the form submission is stopped.

### Booking Validation

The booking page allows the user to select:

- origin
- destination
- travel type
- travel class
- payment mode

Before submission, JavaScript checks that a travel option and the terms-and-conditions agreement have been selected.

### Email Validation

The project performs basic email validation by checking for:

```text
@
.
```

and verifying their relative positions within the entered email address.

### Form Submission

The signup, login, and booking forms are configured to submit using the HTTP `POST` method.

```html
method="post"
```

The forms reference `abcd.html` as their submission target. Since that page and any backend processing are not included in this repository, the project demonstrates the **front-end interaction and validation flow only**, rather than a complete reservation or authentication system.

## Running the Website Locally

This project is a static front-end website, so no application server or database is required.

### 1. Clone the Repository

```bash
git clone https://github.com/as271996/airline-reservation-web-ui.git
cd airline-reservation-web-ui
```

### 2. Open the Home Page

Open the following file in any modern web browser:

```text
air.html
```

You can either:

- double-click `air.html`
- open it from your browser using **Open File**
- use a lightweight local development server

### 3. Optional: Run with a Local Server

If Python is installed, you can start a simple local HTTP server from the project directory.

For Python 3:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/air.html
```

### 4. Navigate Through the Website

Use the navigation menu to access:

```text
Home
Sign Up
Log In
Flights
Book Now
```

### Note

The project is a front-end prototype only.

The signup, login, and booking forms perform client-side validation, but the repository does not include backend processing, persistent storage, or a functional reservation engine.

## Limitations and Future Improvements

This project was built as a front-end web development exercise and can be extended significantly.

- Add a backend service for user registration, authentication, and booking
- Add a database for storing users, flights, and reservations
- Replace static flight data with dynamically loaded flight information
- Add real booking confirmation and reservation IDs
- Add proper payment processing integration
- Add departure and return date selection
- Add passenger-count selection
- Add seat-selection functionality
- Improve validation using modern JavaScript and HTML5 validation attributes
- Replace browser alert messages with inline validation feedback
- Improve responsiveness for mobile and tablet screens
- Add accessibility improvements for forms and navigation
- Improve visual design and user experience
- Add automated frontend tests
- Replace duplicated page styling with a more structured CSS architecture
- Add backend APIs and connect the forms to real application workflows

## Author

**Amit Singh**

Front-end web development project focused on HTML, CSS, JavaScript, multi-page website structure, and client-side form validation.

- GitHub: [github.com/as271996](https://github.com/as271996)
- LinkedIn: [linkedin.com/in/amit-singh-sp27](https://www.linkedin.com/in/amit-singh-sp27)

## Project Context

This project was created to practice foundational web-development concepts through an airline reservation website prototype.

It demonstrates:

- multi-page website navigation
- HTML form design
- custom CSS styling
- JavaScript-based form validation
- signup and login interfaces
- flight-information presentation
- airline booking-form design
- browser-side user interaction

