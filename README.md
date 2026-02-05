# Integrating With HubSpot I: Foundations Practicum

This repository contains my submission for the **Integrating With HubSpot I: Foundations Practicum**, which is one of the two requirements to earn the **Integrating With HubSpot I: Foundations certification**. The second requirement is passing the certification exam with a score of at least 75%.

The goal of this practicum is to demonstrate the ability to build a basic Node.js integration that interacts with the HubSpot CRM APIs.

📘 Official practicum instructions:  
https://app.hubspot.com/academy/l/tracks/1092124/1093824/5493?language=en

---

## What I Built

I created a **Node.js application** using **Express**, **Axios**, and **Pug** that integrates with the **HubSpot CRM API**.

### Custom Object

- **Object name:** Pet
- **Custom properties:**
  - `name` (string)
  - `type` (string)
  - `age` (number)
- The Pet custom object is associated with the **Contacts** object
- Multiple Pet records were created for testing

### Application Functionality

- **Homepage (`/`)**
  - Sends a GET request to HubSpot to retrieve Pet records
  - Displays all records in a table using a Pug template
  - Shows all custom properties (name, type, age)

- **Form page (`/update-cobj`)**
  - Renders a form to create a new Pet record

- **Form submission**
  - Sends a POST request to HubSpot to create a new custom object record
  - Redirects back to the homepage after successful creation

The application was tested locally by running:

```bash
node index.js
```
