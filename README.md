# FIAP - Pos Tech - Tech Challenge One

## Project Description

The "FIAP - Pos Tech - Tech Challenge One" project is an application developed using Node-RED. The project aims to create a platform where users can log in, register, and assign ratings and comments about movies.

## Features

### User Authentication

- In the Login screen, users provide their credentials (username and password).
- Using a GET request, user data is obtained via API for authentication.
- If the credentials are correct, the user is authenticated and directed to the 'Movies' tab.

#### Node-RED Flow - Login
![Captura de tela 2023-11-29 161126](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/b31a3cc1-5486-417b-abad-5b7adef1f716)

#### Node-RED Screen - Login
![Captura de tela 2023-11-29 161305](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/42f932c5-b7b3-4f58-bf8e-e62cba5cf48d)


### User Registration

- Users without login credentials can register on the registration screen.
- A POST request is used to send the new user's data to the API.
- If the user already exists, a message stating "User already exists." is displayed.
- Upon successful registration, the message "User registered." is shown.

#### Node-RED Flow - Register
![Captura de tela 2023-11-29 161416](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/6c63ea91-4b19-4e8b-a4ee-b54e8167bfa1)

#### Node-RED Screen - Register
![Captura de tela 2023-11-29 161504](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/8874be66-92de-448e-926a-82bb4f03e2dd)

### Movie Registration

- Registered users can choose movies from a list and assign ratings and comments.
- Data is stored in JSON files.
- Using the "G-Sheet Append" node, data is sent to a Google Sheets spreadsheet.
- An automation via Zapier sends an email to the administrator whenever a new movie is registered.

#### Node-RED Flow - Movie
![Captura de tela 2023-11-29 161631](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/286079de-dbb4-4d2e-8034-c355d5dfc735)

#### Node-RED Screen - Movie
![Captura de tela 2023-11-29 161616](https://github.com/laraberns/tech-challenge-one-fiap/assets/133805423/5455d1ff-4147-4bef-9225-df59a8517f60)

This project was developed as part of the technological challenge for the "FIAP - Pos Tech" course. Feel free to contribute, report issues, or suggest improvements. Happy exploring!
