# Cafe Finder Web App

## Overview
A Flask-based web application for discovering and adding cafes with ratings for coffee, WiFi, and power sockets. Users can submit new cafe details through a form, which are stored in a CSV file and displayed on a dedicated cafes page. Built with Bootstrap5 for responsive design and WTForms for secure form handling.

## Features
- Add new cafes via a validated web form with Google Maps URL support.
- View all cafes with ratings (coffee ☕, WiFi 📶, power 🔌) on `/cafes`.
- Responsive UI using Flask-Bootstrap5.
- Data persistence using CSV file (`cafe-data.csv`).
- Form validation for required fields and valid URLs.

## Tech Stack
- **Backend**: Flask, Flask-WTF, Flask-Bootstrap5
- **Forms**: WTForms with StringField, SelectField, URL validation
- **Data**: CSV storage/reading with Python's `csv` module
- **Frontend**: Bootstrap5, Jinja2 templates
- **Validation**: DataRequired, URL validators

## Quick Setup
1. Install dependencies:
2. Run the app:
3. Open `http://localhost:5002`
4. Navigate to `/add` to submit cafes, `/cafes` to view list.

## Routes
| Route | Description | Method |
|-------|-------------|--------|
| `/` | Home page | GET |
| `/add` | Add new cafe form | GET/POST |
| `/cafes` | View all cafes list | GET |

## File Structure
project/
├── main.py # Flask app, forms, routes, CSV handling
├── cafe-data.csv # Cafe data (auto-created)
├── templates/
│ ├── index.html
│ ├── add.html
│ └── cafes.html
└── README.md # This file
