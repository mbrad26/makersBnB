# makersBnB

# Headline specifications

* Any signed-up user can list a new space.
* Users can list multiple spaces.
* Users should be able to name their space, provide a short description of the space, and a price per night.
* Users should be able to offer a range of dates where their space is available.
* Any signed-up user can request to hire any space for one night, and this should be approved by the user that owns that space.
* Nights for which a space has already been booked should not be available for users to book that space.
* Until a user has confirmed a booking request, that space can still be booked for that night.

# Nice-to-haves

* Users should receive an email whenever one of the following happens:
* They sign up
* They create a space
* They update a space
* A user requests to book their space
* They confirm a request
* They request to book a space
* Their request to book a space is confirmed
* Their request to book a space is denied
* Users should receive a text message to a provided number whenever one of the following happens:
* A user requests to book their space
* Their request to book a space is confirmed
* Their request to book a space is denied
* A ‘chat’ functionality once a space has been booked, allowing users whose space-booking request has been confirmed to chat with the user that owns that space
* Basic payment implementation though Stripe.

# MVP 

Owner can list one or more spaces. / 
Owner can add space with name, description and ppn. /
Owner should be able to offer a range of dates where their space is available.

Holiday maker can view spaces. /
Holiday maker can click on individual space for more information. /
Holiday maker can click on individual space to make enquiry 

# User Stories

As a user, so I can sign up
I would like a sign up page to store name, pwd, email

As a user, so i can see all the listings, 
I would like to see a list of all spaces

As a user, so I can post my space(s), 
I would like to submit my listing with a name, description, ppn and dates 

As a user, so I can see more information on the space,
I would like to click on a specific listing

As a user, so I can make an enquiry, 
I would like to email the space owner

# Domain Model

# CRC

# Agreed working day
(i.e. stand-ups/ pull requests/ retros)

CREATE TABLE listings(id SERIAL PRIMARY KEY, name VARCHAR(60), description VARCHAR(280), price DECIMAL(6, 2), created_at TIMESTAMP);

