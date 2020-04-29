## GoBarber

GoBarber is a practice application built using React, React Native and Node.js.
It is currently a work in progress.

### Instructions

Since only the backend is available so far, you'll need to use a tool to interact with it, such as Insomnia or Postman.

- cd backend
- yarn install

At this point the server should be running.

You can create an appointment (in preparation for when users select theri barber and create an appointment), or list all appointments.

- Create appointment:
  - hit this url: GET http:localhost:3000/appointments
  - body:
    {
    "provider_id": pass the user ID generated from create user url here as string,
    "date": "{% now 'iso-8601', '' %}"
    }
- List appointment:
  - hit this url: POST http:localhost:3000/appointments

You can also create a user (in preparation for a login)

- Create user:
  - hit this url: POST http:localhost:3000/users
  - body:
    {
    "name": "Thales Kenne",
    "email": "youremail@gmail.com",
    "password": "123456"
    }
