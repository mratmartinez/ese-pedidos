# Ese Pedidos

##### DISCLAIMER: This project was meant to go live in my city, as there's nothing similar there. Due to personal issues I was unable to do this. Therefore I decided to upload it to GitHub so it wouldn't go to waste. It is NOT intended to be a general purpose solution, it was something that made sense under a very specific context (a small city).

This project is meant to facilitate ordering food from restaurants. Instead of calling or texting a specific number for ordering food you have an app with a list of restaurants to choose from.

### This has some advantages:
* You don't need to have as many numbers in your agenda to call. In fact, you don
* You get the full restaurant menu, with descriptions and prices.
* You can order from restaurants you didn't know of, trying new food!
* Since phone numbers are verified, you have the possiblity to ban numbers that make fake orders.

# How would it work?

There are 2 apps, one for the clients and another one for the restaurants.

On the clients app, you will be presented with a choice of restaurants. After picking one, you can then select what food you will order and the delivery destination. Upon issuing an order. it will be marked as 'Pending', this means you have to to wait until the restaurant processes (i.e, confirms) your order.

Once your order is confirmed by the restaurant, you only have to wait for it to be delivered to the location you specified earlier. The payment is made when the order arrives.

# Features

### Statistics for restaurants


### Restaurant Fees
My idea for monetizing this project was to charge restaurants a small fee (say 5%) on every order. 

### Location on map
Aside from the address, the clients are required to submit the delivery location when issuing an order. This is easily done with the Maps API. Just a few taps.

### Chat
When you make an order, a chat between the client and the restaurant is created. This chat is specific to the order.\
This is useful in the following scenario: A restaurant

# Frameworks Used

### Frontend:

Angular 4\
SocketIO\
Ionic 2\
Google Maps JS

### Backend

Flask\
Flask SocketIO\
SQLAlchemy
MariaDB (on live demo server)

# Live Demo

[Clients App](http://siwka.net/ese-pedidos/client)\
[Restaurants App](http://siwka.net/ese-pedidos/restaurant)

# Things that don't work

## Phone verification
I originally intended to send an SMS with a code to the phone being verified and make the user enter this code on the app. Since sending SMS is a paid service and there are many providers with different implementations, I decided to skip this. This means you can just log in with any phone number and it will work as if it was a different client account. You'll have to implement this yourself.

## Changing the logo of a restaurant
TODO

# Building
### Client/Restaurant Apps
Make sure you have npm installed

If you don't, install it:
>sudo npm -g install cordova ionic

Then just go to any app folder (either client or restaurant) and run this command to build and test:
>ionic serve --lab

NOTE: The first build may take a few minutes, if you get a prompt to install 

### Server
Install python dependencies:

Now the only thing left to do is to configure the db.\



