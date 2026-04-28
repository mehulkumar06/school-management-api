# School Management API

This project is a Node.js REST API built using Express.js and MySQL for managing school data.

## Features
- Add new schools to the database
- Retrieve schools sorted by proximity to user location
- Distance calculated using Haversine formula

## Tech Stack
- Node.js
- Express.js
- MySQL

## API Endpoints

### Add School
POST /api/addSchool

Example body:
{
"name": "Delhi Public School",
"address": "Delhi",
"latitude": 28.7041,
"longitude": 77.1025
}

### List Schools
GET /api/listSchools?latitude=28.70&longitude=77.10

Returns schools sorted by distance from the user.

## Setup Instructions

1. Clone the repository

git clone https://github.com/mehulkumar06/school-management-api.git

2. Install dependencies

npm install

3. Start server

npm run dev