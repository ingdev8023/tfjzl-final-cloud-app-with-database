# Django Online Course App with Database

Final project for the IBM/Coursera course **Django Application Development with SQL and Databases**.

This project is a Django web application for an online course platform. It includes course listings, user registration and authentication, course enrollment, lessons, exam questions, answer choices, submissions, and exam result calculation.

## Project Overview

The application provides a basic online learning platform where users can:

- Register and log in
- View available courses
- Enroll in a course
- Access course lessons
- Submit answers to course assessment questions
- View exam results after submission

The final project extends the provided `onlinecourse` Django app by adding an assessment feature connected to the database.

## Tech Stack

- Python
- Django
- SQLite
- HTML
- CSS
- Bootstrap
- JavaScript
- Git / GitHub

## Main Features

### User Authentication

Users can register, log in, and log out using Django's built-in authentication system.

### Course Management

The app includes course, lesson, instructor, learner, and enrollment models. Courses can contain multiple lessons and can be associated with multiple instructors.

### Enrollment System

Authenticated users can enroll in available courses. Each enrollment connects a user with a course and stores enrollment-related data.

### Assessment Feature

The assessment feature allows courses to include questions and multiple answer choices.

The main assessment models are:

- `Question`
- `Choice`
- `Submission`

A learner can submit selected choices for a course assessment, and the app calculates the final score based on correct answers.

### Exam Result Calculation

After submitting an exam, the application compares the learner's selected choices with the correct choices for each question and calculates the final grade.

## Database Models

The project includes the following main models:

- `Instructor`
- `Learner`
- `Course`
- `Lesson`
- `Enrollment`
- `Question`
- `Choice`
- `Submission`

These models define the relationship between users, courses, lessons, enrollments, and assessments.

## Project Structure

```text
.
├── manage.py
├── myproject/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── onlinecourse/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── admin.py
│   ├── migrations/
│   └── templates/
├── static/
├── requirements.txt
├── Procfile
├── manifest.yml
└── runtime.txt
