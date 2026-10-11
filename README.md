# E-Kalusugan System

A web-based health records system for the **Barangay San Isidro Health Center**, built as a Performance Task for CPE Laws.

The whole app is a single `index.html` file. It runs entirely in the browser and keeps its data in the browser's `localStorage`, so it needs no server or database.

## Features

- **Login and registration**: users sign in before they can see any records. Passwords are stored as salted SHA-256 hashes, never as plain text.
- **User roles**
  - **Administrator**: full access, including user management and dispensing medication.
  - **Health Worker**: day-to-day access to patients, consultations, programs and inventory.
- **Dashboard**: an overview of patients, consultations and medicine stock.
- **Patient Records**: register residents and search the patient list.
- **Consultations**: log check-ups for registered patients.
- **Barangay Health Programs**: Immunization (Bakuna), Maternal & Prenatal, Senior Citizens, and TB-DOTS.
- **Pharmacy & Inventory**: track medicine supplies from the DOH and Municipal Health Office, and dispense medication (admin only).
- **User Management** (admin only): add or delete accounts and switch users between Administrator and Health Worker.

## How to Run

1. Download or clone this repository.
2. Open `index.html` in a web browser.

You can also use the GitHub Pages site if one is set up for this repository.

### Default Admin Account

| Username | Password   |
|----------|------------|
| `admin`  | `admin123` |

The app creates this account the first time it runs. New accounts made from the Register tab are Health Worker accounts. An admin can promote them under **User Management**.

## Notes

- Data is saved only in the browser you are using. Clearing browser data or switching to another browser or computer starts over with the sample data.
- This is a school project and a demonstration. It is not meant to store real patient information.

## Tech Stack

- HTML, JavaScript
- [Tailwind CSS](https://tailwindcss.com/) (CDN)
- [Font Awesome](https://fontawesome.com/) icons
