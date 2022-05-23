# Trading-Schedule-Public

This is an internal tool that I built for Caesars Sportsbook.

This is a scheduling tool. It pulls in all of the different games that we offer for a variety of sports and assigns traders to those games. Traders can view their own schedule, filter by date, keyword, or league.

When a trader goes to their page, stats are given on the bottom and they can access their "trader dashboard" (still in development).

There are a number of other features to this application. Below, you'll find multiple screenshots and video walk-throughs of everything the application can do.

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

### 4. Refresh table

![refresh_table](https://user-images.githubusercontent.com/93163082/169715428-2c5745ac-16a9-48ee-abaa-98d5f3c8b62c.gif)

### 5. League Filters (these filters won't be affected by the "Refresh" button)

  Step 1: Click arrow in upper right corner of screen
  
![leagues1](https://user-images.githubusercontent.com/93163082/169716133-efa9516b-447e-4636-ace8-cf9dff88c5c6.png)

  Step 2: On left top of screen, Choose Sport > Country > League

![leagues2](https://user-images.githubusercontent.com/93163082/169716256-f2df8c17-3b22-4cb0-bc1d-10b189283a6e.png)

![leagues3](https://user-images.githubusercontent.com/93163082/169716261-63ed2bb2-42ed-4cc0-8e37-8258f26f5870.png)

![leagues4](https://user-images.githubusercontent.com/93163082/169716268-a62b3fbe-8cf2-4683-80e3-dbdde128bb21.png)

  Step 3: Click "Filter" button on right side of screen
  
![leagues5](https://user-images.githubusercontent.com/93163082/169716276-f0702923-da90-4f89-a8ce-48591f0a20ac.png)

![leagues6](https://user-images.githubusercontent.com/93163082/169716278-93335281-8249-48c0-98a5-0cc6a3101987.png)

### 6. Game Details on click + hover

![game_details](https://user-images.githubusercontent.com/93163082/169716428-7db711e3-b9f1-4b20-8abd-5cbfed5c30ff.gif)

### 7. Duplicates Button (filters table to show only the games that are listed twice, once by each feed provider)

![duplicates](https://user-images.githubusercontent.com/93163082/169871690-e51d0ae5-ccc4-4695-b69f-9fc13e962cc7.gif)

### 8. Notifications (a notification will be shown for any game without a trader attached to it. When a trader is attached, the notification will go away)

![notifications](https://user-images.githubusercontent.com/93163082/169872424-f0944c36-a3af-402b-9571-181ddbc90b07.gif)

### 9. Trader Stats and Dashboard (still in development)

![trader_stats](https://user-images.githubusercontent.com/93163082/169872908-6dd6f140-758a-41b2-86aa-b0cbbae05263.gif)




