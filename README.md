# Trading schedule

An internal tool I built for the Caesars Sportsbook trading floor in Las Vegas (2018 to 2022). This repository is a write-up; the code belongs to the sportsbook. Case study: [scottbarclay.dev/work/trading-schedule](https://scottbarclay.dev/work/trading-schedule).

## What it did

A sportsbook trades hundreds of games a day across dozens of leagues, and each one needs a trader watching it. The first tool I ever built for the desk was a Python script that gave every matchup a proper ID and mapped it to a trader. This is what it grew into: a scheduling app that pulled every upcoming game from the book's two data feeds and assigned a trader to each one, so nothing went live without an owner.

## How it worked

- Games came from the BetRadar and BetGenius feeds (the two providers the book bought its fixtures from), pulled with Axios on the server and rendered into one table.
- Traders were assigned by their shifts and the leagues they covered. Each trader had a page showing their own games, with stats at the bottom.
- Any game with no trader attached showed a notification until someone took it.
- Both feeds list many of the same games under different IDs, so a duplicates view showed only the games listed twice, one per feed, for reconciling by hand rather than trading twice.
- Filters by date, keyword, and league (sport, then country, then league).

Stack: Node, Express, MySQL, the two feed APIs.

## Screens

Home:

![Home screen](https://user-images.githubusercontent.com/93163082/169713029-5ebd3564-bc1a-432f-801f-53b1d80c54ee.png)

A trader's own schedule:

![Choose trader](https://user-images.githubusercontent.com/93163082/169714710-533996f0-4629-4f38-99fe-67a4f22c06d8.gif)

Reassigning a game:

![Change trader](https://user-images.githubusercontent.com/93163082/169714868-bde8eb2c-b5ec-4a50-8e95-9505e8759316.gif)

Unowned-game notifications:

![Notifications](https://user-images.githubusercontent.com/93163082/169872424-f0944c36-a3af-402b-9571-181ddbc90b07.gif)

Duplicates across the two feeds:

![Duplicates](https://user-images.githubusercontent.com/93163082/169871690-e51d0ae5-ccc4-4695-b69f-9fc13e962cc7.gif)

Game details:

![Game details](https://user-images.githubusercontent.com/93163082/169716428-7db711e3-b9f1-4b20-8abd-5cbfed5c30ff.gif)
