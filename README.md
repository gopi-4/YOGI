# YOGI
  - [YOGI](https://gopi-4.github.io/YOGI/) is a single page responsive application.
  - At home you see all registered users. And to register fill the application form.
  - Frontend validation checks on Input fields (i.e on dob(18<=age<=65), email, name, slot) gives error on invalid input.
  - User get registered only if he/she is not registered for the given month else gives error. 
  - Once the user registered, past entry of user if present gets deleted to save space. 

## Work Flow
![work_flow](https://user-images.githubusercontent.com/78689282/206988995-b81514c5-b65c-41b5-86f1-2871e8e1da20.jpg)

## Schema Description
### User
| Attribute | Type | Nullable | Description |
| :--- | :--- | :--- | :--- |
| Id | Integer | NO | Primary Key |
| name | String | NO | User name |
| email | String | NO | User email |
| dob | String | NO | YYYY/MM/DD |
| phone | String | YES | 10 digits mobile no. |
| slot | String | NO | 1, 2, 3 or 4 |
| registration_date | String | NO | date at which user registered |
| payment_status | Boolean | NO | payment status |

## API Description

### Base URL : https://yog-backend-production.up.railway.app

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/9a7f96e52b0831af3cb2?action=collection%2Fimport)

### 1. `/api/getUsers`
- `GET`: Get all user

### 2. `/api/registerUser`
- `POST`: Create a new user
    - Request Body:
        | Parameter | Type | Required | Description |
        | --------- | ---- | -------- | ----------- |
        | name | string | yes | user name |
        | email | string | yes | unique email |
        | phone | string | No | 0-10 digits long |
        | dob | string | yes | YYYY/MM/DD Format |
        | slot | string | yes | 1, 2, 3 or 4 |
        
## ER Diagram
![ERD](https://user-images.githubusercontent.com/78689282/206994144-dc060b49-b33b-40dd-ab62-ed54cc637ed5.jpg)

## Testing Credentials
| Purpose | Test Email |
|--|--|
| successful transaction | example@mail.com  |
| unsuccessful transaction | test_payment_fail@gmail.com |

## Tech Stack
<img src="https://img.shields.io/badge/React%20-%20Js-blue" > <img src="https://img.shields.io/badge/Spring%20-Boot%20-brightgreen" > <img src="https://img.shields.io/badge/Free-%20SQL-orange" > 

## Getting Started 
### Setup the repository to your local environment.

  ```git
  Fork repo
  git clone https://github.com/YOUR-USERNAME/YOGI
  cd YOGI
  ```
  ## Frontend Setup
  ```sh
  cd frontend/yoga-class-form
  npm install
  npm start
  ```

  ## Backend Setup
  ```sh
  cd backend/yoga
  mvn spring-boot:run (Note: make sure you have maven installed)
                               or
                           run on IDE
  ```

## Hosting
  - Frontend :- [github-pages](https://pages.github.com/)
  - Backend  :- [railway](https://railway.app/)
  - Database :- [freesqldatabase](https://www.freesqldatabase.com/)
  
## Authors

- [@GaneshKalyankar](https://www.linkedin.com/in/gkalyankar)

 <center> <p align="center">--- Enjoy Coding --- </p></center>
