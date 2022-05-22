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

![choose_trader](https://user-images.githubusercontent.com/93163082/169714710-533996f0-4629-4f38-99fe-67a4f22c06d8.gif)




## Features



### 1. Edit Traders Assigned to games

![change_trader](https://user-images.githubusercontent.com/93163082/169714868-bde8eb2c-b5ec-4a50-8e95-9505e8759316.gif)

### 2. Filter by Date

![date_filter](https://user-images.githubusercontent.com/93163082/169715010-25687427-7922-45be-abeb-b6cc405ae947.gif)

### 3. Search by Keyword

![search_filter](https://user-images.githubusercontent.com/93163082/169715362-83b72097-2642-4dd6-abf1-e0b8e6e4ebd0.gif)










