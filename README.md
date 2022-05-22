# Trading-Schedule-Public
Public repo for Trading Schedule

This is an internal tool that I built for Caesars Sportsbook.

Below, you'll find multiple screenshots and video walk-throughs of the application.

Enjoy!


## Home Screen


![home_screen](https://user-images.githubusercontent.com/93163082/169713029-5ebd3564-bc1a-432f-801f-53b1d80c54ee.png)

### Where does the match data come from?
The data is being pulled in using API's from BetRadar and BetGenius. I'm using axios on the server side to make these requests, and sending that data to the client side.
I am then parsing that data and appending it to the table you see.

### How are traders assigned?
Traders are assigned based on their schedules and the Leagues they have been assigned.

### How do traders view their personal schedule?


