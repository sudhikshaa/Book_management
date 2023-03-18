# Book_management


Server >> Storing certain data
       >> User Register
       >> Subscriber


This is a Book Record MAnagement API Server / Backend for the library system or management of certain records or manuals or books

Fine System
User : 06/03/2023  - 06/06/2023
He/She came by 06/05/2023  ->50
               09/05/2023  ->150
               
Subscriptions 
  3 months (Basic)
  6 months (Standard)
  12 months (Premium)
  
If the subscription type is standard && if the subscription date is 06/03/2023
=> the subscription valid till 06/09/2023

within subscription date >> if we miss the renewal >> 50/- per day
subscription date is also been missed >> and also missed the renewal >> 100 + 50/- day


>> book1
>> basic
>> 06/03/2023 -> subscription date
>> 07/03/2023 -> borrowed a book from library
>> book1 renewal date is on 21/03/2023
>> 23/03/2023 -> we need to pay an fine of 50*2 - 100/-


>> book2
>> basic
>> 06/03/2023 -> subscription date
>> 07/03/2023 -> borrowed a book from library
>> book2 renewal date is on 21/03/2023
>> 23/06/2023 -> we need to pay a fine of 100+(no of day * 50)


>> missed by renewal date >> 50/-
>> missed by subscription date >> 100/-
>> missed by renewal & subscription date >> 150/-




# Routes and Endpoints

## /users
POST : Create a new user 
GET  : Get all the user information here

## /users/{id}
GET : Get a user by ID
PUT : Update a user by their ID
DELETE : Delete a user by ID (Before deleting check he/she still have an issued book) && (is there any fine to be payed)

## /users/ subscription-details/{id}
GET : Get user subscription details 
         >> Date of subscription
         >> Valid till
         >> Is there any fine
         
## /books
GET : Get all the books
POST : Create / Add a new book

## /books/{id}
GET : Get a book by ID
PUT : Update a book by ID



## npm init
## npm i nodemon --save-dev
## npm install express
## npm run dev
