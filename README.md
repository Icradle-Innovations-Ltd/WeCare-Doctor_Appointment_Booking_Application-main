# Doctor Appointment Booking Application

## A Doctor's Appointment Booking System
A system that lets you register and login to view doctors, book appointments, view/reschedule and delete appointments.

### Note
As the backend is deployed using Render, there may be longer than expected delays. We apologize for any inconvenience.

## Credentials

### Patient Login Credentials
- Email: `user1@gmail.com` | Password: user1
- Email: `user2@gmail.com` | Password: user1
- Email: `patient11@gmail.com` | Password: patient11

### Doctor Login Credentials
- Email: `doc1@gmail.com` | Password: doc1 (has existing appointments)
- Email: `pococare@gmail.com` | Password: pococare

### Video Call Feature Note
To try the video call feature, please register with your real email as a Doctor and log in with any of the above patient credentials. This is required as Nodemailer cannot send emails to dummy email addresses.

## Features
* Authentication using JWT tokens
* Doctor and Patient registration/login
* Secure logout using blacklist
* Patient appointment management (book, edit, delete)
* Real-time video consultations
* Doctor availability toggle
* Email notifications for video call links

## Application Flow

* Registration (Patient/Doctor)
* Patient Features
   * View all doctors
   * Book appointments
   * Modify/delete appointments
   * Start video calls (when doctor is available)
   * Video chat in private rooms
   * Video/audio controls
* Doctor Features
   * Manage video call availability
   * View booked appointments
* Secure logout

## Tech Stack
[![My Skills](https://skillicons.dev/icons?i=js,nodejs,express,mongodb,html,css)](https://skillicons.dev)

## Tools
[![My Skills](https://skillicons.dev/icons?i=vercel,github)](https://skillicons.dev)
![NPM](https://www.w3schools.com/whatis/img_npm.jpg)

## Links
- [Live Demo](https://wecareyou.vercel.app/)
- [Backend API](http://localhost:3000/)

## Screenshots

### Home Page
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/fc64ac55-26d5-438f-ba2c-39c75b6e5aa8)

### Login Page
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/791a559d-0908-40f4-aefd-90867e8383d5)

### Doctor View
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/52f852c3-191b-4473-8f3f-08f79d99e14c)

### Patient View
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/f30893d8-d55d-4e89-a487-1fa42342c0ef)

### Patient Dashboard
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/43c24b4a-126b-4e0c-8345-f0aa88927182)

### Appointments Management
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/7ae53a8b-c630-4b98-b46f-d2253919d7de)
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/e186ba87-2a4d-4658-be90-343b6d99cf75)

### Video Consultation
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/76f9def2-1602-4b13-8b22-2d6f60ea1405)

### Video Call Room
![image](https://github.com/DhaanuI/Pococare_assignment/assets/112754832/b0efab74-d38d-4d54-8245-a108fa33588c)

## Installation Guide

1. Clone the repository: [Pococare Assignment](https://github.com/DhaanuI/Pococare_assignment)
2. Open in VS Code
3. Install dependencies: `npm install`
4. Navigate to backend: `cd backend`
5. Start server: `npm run server`

## API Endpoints

Base URL: `http://localhost:3000/`

| METHOD | ENDPOINT | DESCRIPTION | STATUS CODE |
| --- | --- | --- | --- |
| POST | api/patients/signup | Patient registration | 201 |
| POST | api/patients/login | Patient login | 201 |
| PATCH | api/patients/update/:id | Update patient | 200 |
| DELETE | api/patients/delete/:id | Delete patient | 200 |
| GET | api/patients/all | Get all patients | 200 |
| POST | api/patients/logout | Patient logout | 200 |
| POST | api/doctors/signup | Doctor registration | 201 |
| POST | api/doctors/login | Doctor login | 201 |
| PATCH | api/doctors/update/:id | Update doctor | 200 |
| DELETE | api/doctors/delete/:id | Delete doctor | 200 |
| GET | api/doctors/all | Get all doctors | 200 |
| POST | api/doctors/logout | Doctor logout | 200 |
| GET | api/appointments/ | Get all appointments | 200 |
| POST | api/appointments/add | Create appointment | 201 |
| PATCH | api/appointments/update/:id | Update appointment | 200 |
| DELETE | api/appointments/delete/:id | Delete appointment | 200 |
| GET | api/appointments/docapp/:id | Get doctor appointments | 200 |
| GET | api/appointments/patapp/:id | Get patient appointments | 200 |

Thank you for your time!
