# Fractions Calculator

## Overview

This is a Node.js application using Express and Handlebars (hbs) as the templating engine. The application allows users to perform operations on fractions, such as:

- Simplifying a fraction
- Adding two fractions
- Adding multiple fractions

## Features

- Express.js backend for routing and serving pages.
- Handlebars (hbs) as the templating engine for rendering dynamic pages.
- JavaScript-based calculations for handling fractions, including GCD-based simplification and addition.

## Project Structure

```text
fractions/
├── src/
│   ├── app.js                           # Express server configuration
├── templates/
│   ├── views/
│   │   ├── index.hbs                    # Simplify fractions page
│   │   ├── addFractions.hbs             # Add two fractions page
│   │   ├── addFractionsArray.hbs        # Add multiple fractions page
│   ├── partials/
│       ├── header.hbs
│       ├── footer.hbs
├── public/
│   ├── css/
│   │   ├── styles.css                   # Stylesheets for UI
├── package.json                         # Project dependencies & scripts
├── README.md                            # Documentation
```

## Installation

### Prerequisites

- Node.js (v16 or later recommended)
- npm (Node Package Manager)

### Steps to Install

1. Clone the repository:

   ```sh
   git clone https://github.com/Vipin-1999/Fractions.git
   cd Fractions
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

## Running the Application

To start the server in development mode:

```sh
npm start
```

This will start the Express server on `http://localhost:3000`.

## Endpoints

### Home (`/`)

- **Renders**: `index.hbs`
- **Description**: Page for simplifying fractions.

### Add Two Fractions (`/addFractions`)

- **Renders**: `addFractions.hbs`
- **Description**: Allows users to enter two fractions and calculate their sum step-by-step.

### Add Multiple Fractions (`/addFractionsArray`)

- **Renders**: `addFractionsArray.hbs`
- **Description**: Allows users to enter multiple fractions and compute their sum iteratively.

## Dependencies

The project uses the following Node.js packages:

- `express` - Web framework for Node.js
- `hbs` - Handlebars templating engine
- `path` - Path utilities
- `nodemon` - Development tool for auto-restarting the server
- `bootstrap` - Frontend styling framework
- `jquery` - JavaScript library for DOM manipulation
- `request` - HTTP request library (not currently used but installed)
