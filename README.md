# AireAppointments — Workshop Challenge

This is a fun coding challenge — see how far you can get! There are no right or wrong answers; the aim is to have a go, learn something new, and build something you can be proud of.

## Overview

AireAppointments is a fictional healthcare technology company operating in West Yorkshire. Currently, all appointments are managed over the phone and manually entered by a practice receptionist.
AireAppointments would like to automate this process.

## Aims

1. Build a patient appointment booking system
2. Create a patient facing form for appointments
3. Build a simple practice admin area behind a login screen
4. Display appointments in a table view ordered by date
5. Provide functionality to edit and approve appointments

## Approaches — Pick What Interests You

This challenge is flexible — you don't have to build everything. Choose the angle that excites you most:

### 🖥️ Focus on the Backend

Build an API or server-side app that handles appointment data. You don't need a polished UI — even returning JSON from a few endpoints is great.

- Store data however you like: in memory (data resets on restart, which is fine!), a text file, SQLite, or a full database
- You can test your endpoints with a tool like [Postman](https://www.postman.com) or [Hoppscotch](https://hoppscotch.io) instead of building a UI

### 🎨 Focus on the Frontend

Build the forms and admin screens as a web interface. You don't need a real backend — just keep the appointment data in memory in your app (e.g. a JavaScript array). The data will disappear on page refresh, and that's completely fine.

- Use plain HTML/CSS/JavaScript, or a frontend framework like **React**, **Vue**, **Svelte**, or **Angular**
- React is the most widely used in industry right now, but all of these are great choices

### 🔗 Go Full Stack

Build both a frontend and a backend that talk to each other — the full picture. This is the most challenging path but also the most satisfying if you get it working.

> There's no pressure to do everything. A focused, working slice is great — but so is an ambitious attempt at the whole thing, even if not everything is finished!

## Technology Requirements

### Language

Use whatever language you feel comfortable with — there's no wrong choice here! If you're not sure where to start, we'd recommend:

- **Python** — great for beginners and widely used in industry
- **.NET (C#)** — solid choice for building web applications

Other modern options that work well for this kind of project include **Node.js**, **Go**, or **Java** — feel free to use any of these if you're already familiar with them.

### Data Storage

Your app needs somewhere to store appointment data. Pick whatever level you're comfortable with:

| Option                                  | Good for...                                                                   |
| --------------------------------------- | ----------------------------------------------------------------------------- |
| A **text file** (e.g. `.txt` or `.csv`) | Getting started quickly without a database                                    |
| **SQLite**                              | A simple database stored as a single file — no server setup needed            |
| **PostgreSQL**                          | A powerful, industry-standard database — great to try if you want a challenge |
| **MySQL / MSSQL**                       | Other popular databases, also perfectly fine                                  |

Don't worry if you've never used a database before — a text file or SQLite are completely valid and a great place to start.

### Nice to Have

- Styling with a UI framework — pick whichever looks appealing to you:
  - **Bootstrap** — beginner-friendly, lots of examples online
  - **Tailwind CSS** — very popular in modern web development
  - **Material UI** — Google's design system, great with React
  - **Bulma**, **Pico CSS**, or any other framework you'd like to explore
- Containerised setup (e.g. Docker / Docker Compose)
- Unit tests — don't worry if you haven't written tests before, but if you'd like to give it a go, here are some frameworks to look at based on your chosen language:
  - **JavaScript / TypeScript** — [Vitest](https://vitest.dev) (recommended for modern projects) or [Jest](https://jestjs.io)
  - **Python** — [pytest](https://pytest.org) (very beginner-friendly)
  - **.NET (C#)** — [xUnit](https://xunit.net) or [NUnit](https://nunit.org)
  - **Java** — [JUnit](https://junit.org)
  - **Go** — testing is built into the language with the `testing` package

## Patient Facing Form

Create a simple form that submits and saves appointment data to a database. This data will be used in the admin area.

### Required Fields

- **Name** (required)
- **Appointment Date and Time** (required)
- **Desc** (required)
- **Contact Number** (required)
- **Email Address** (required)

## Admin Area

The admin area should be protected behind a login system.

### Authentication

- Login form must include:
  - Email Address
  - Password
- A registration flow is **not required**
- Credentials should be stored in the database
- You may:
  - Manually insert a user into the database
  - Or create a seeder to populate a user during setup

## Admin Features

### Appointments Table

- A simple table listing all appointments
- Ordered by appointment date
- Columns should match the patient form fields

### Actions Column

Each row should include:

- **Approve**
  - Tick icon or button
  - When approved, the row should change colour
- **Edit**
  - Opens an edit screen
  - Form contains the same fields as the patient form
  - Fields are pre populated
  - Changes should save and reflect in the table
- **Delete**
  - Removes the appointment

### Navigation

- Include a navigation bar
- Provide a logout option

## Source Control

- We recommend hosting your project on a **public GitHub repository** so you can show off your work
- Try to commit as you go after completing each feature
- A clear commit history is a great way to show your progress

## Additional Notes

- Try to make your solution:
  - Functional for users
  - Readable and maintainable for other developers
  - Easy to extend in the future

- Feel free to use AI coding tools if you'd like — we just encourage you to be ready to talk through the decisions you made along the way

- Aim to meet the core requirements rather than over-engineer
