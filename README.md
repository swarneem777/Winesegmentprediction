# Customer Segment Prediction App

The Customer Segment Prediction App is a web application that allows users to predict the customer segment for a new wine based on a wine shop dataset. The prediction is made using Principal Component Analysis (PCA) and machine learning techniques.


## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)

## Introduction

The Customer Segment Prediction App is designed to provide insights into wine consumer behavior by predicting the customer segment for a new wine. The app uses a wine shop dataset and applies PCA to extract meaningful features from the data. Machine learning algorithms are then utilized to predict the customer segment based on the provided wine attributes.

## Features

- User authentication: Users can register and log in to the app using their email and password.
### Login Page:

![Login Page](./Screenshot/Login.png)

### Register Page:

![Register Page](./Screenshot/Register.png)
- Attribute form: Logged-in users can enter wine attributes for prediction. There are 13 attributes.
![Attribute Page](./Screenshot/Attribute-1.png)
![Attribute Page](./Screenshot/Attribute-2.png)


- Prediction: The app uses machine learning models to predict the customer segment based on the provided wine attributes.
![Prediction](./Screenshot/Prediction.png)

- Logout: Users can log out of the app when they are finished.
![Prediction](./Screenshot/Logout.png)


## Technologies

The following technologies are used in this project:

- **Front-end**: React.js
- **Back-end**: Node.js
- **Data Science**: Python, scikit-learn
- **Styling**: CSS
- **Database**: Local storage (browser)

## Installation

To run the Customer Segment Prediction App locally, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/customer-segment-prediction-app.git`
2. Navigate to the project directory: `cd customer-segment-prediction-app`
3. Install the dependencies:
   - For the front-end:
     - Navigate to the `client` directory: `cd client`
     - Run `npm install`
   - For the back-end:
     - Navigate to the `server` directory: `cd server`
     - Run `npm install`
4. Start the development server:
   - For the front-end: Inside the `client` directory, run `npm start`
   - For the back-end: Inside the `server` directory, run `npm start`

## Usage

1. Open your web browser and go to `http://localhost:3000` to access the Customer Segment Prediction App.
2. If you are a new user, click on the "Register" button to create an account. Provide your full name, email, and password.
3. If you already have an account, click on the "Login" button and enter your registered email and password.
4. Once logged in, you will be directed to the Attribute Form page. Enter the wine attributes in the provided input fields.
5. Click on the "Predict" button to submit the form and receive the predicted customer segment for the new wine.
6. To log out, click on the "Logout" button.

## API Documentation

The Customer Segment Prediction App utilizes a local storage-based API for user authentication and storing registration data. The API endpoints are as follows:

- `POST /register`: Register a new user. Payload should include `name`, `email`, and `password`.
- `POST /login`: Log in a user. Payload should include `email` and `password`.
