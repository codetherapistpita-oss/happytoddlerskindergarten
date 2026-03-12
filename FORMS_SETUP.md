# Form Setup Guide

The **Contact** and **Appointment** forms use [Formspree](https://formspree.io) to send submissions to your email — no backend server needed.

## Quick Setup (5 minutes)

### 1. Create a Formspree account
- Go to [formspree.io](https://formspree.io)
- Sign up (free)

### 2. Create two forms
- **Form 1 – Contact:** For the Contact page (general inquiries)
- **Form 2 – Appointment:** For enrollment/appointment requests

### 3. Get your Form IDs
After creating each form, Formspree gives you a URL like:
```
https://formspree.io/f/abc123xyz
```
The Form ID is the part after `/f/` (e.g. `abc123xyz`).

### 4. Update the website

**Contact form** — In `contact.html`, replace `YOUR_CONTACT_FORM_ID` with your **Contact** Form ID:
- `contact.html` (around line 127)

**Appointment form** — In `index.html` and `appointment.html`, replace `YOUR_APPOINTMENT_FORM_ID` with your **Appointment** Form ID:
- `index.html` (around line 511)
- `appointment.html` (around line 101)
- `classes.html` (around line 355)

Search for `YOUR_CONTACT_FORM_ID` or `YOUR_APPOINTMENT_FORM_ID` and replace with your actual Formspree form ID.

### 5. Verify
Submit a test message on your live site. You should receive it at the email linked to your Formspree account.

---

**Free tier:** 50 submissions per month. Upgrade if you need more.
