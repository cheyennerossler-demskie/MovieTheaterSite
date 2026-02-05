# MovieTheaterSite
Senior Project, SUNY New Paltz

## Link to Project
https://github.com/ecarpouzis/MovieTheater.git
- Flatbox Studios Supervisor: Eric Carpouzis

## Purpose
MovieTheater is a website to celebrate cinema and combat the endless options on streaming services. This web application is a tool to track movies we have access to watch, we can mark if a movie has been seen already or if we want to watch it, and we can easily making decisions about movie night by discovering our friend's updates as well! 

This site was first built in ASP.Net MVC, then migrated to .Net Core. A new front-end driven by React is currently underway, and can be seen in the React branch.

## Features
Movie Data & Posters - Data has been retrieved through various methods including web scraping and API access. Posters were once stored as BLOBs, but I found it faster and less resource-intensive to store them as files. When a new movie is added to the site a Python script is ran to create a high quality/small sized thumbnail, which is used when browsing for movies.

Users - A typical ASP.Net Identity implementation would be trivial, but this site is communally shared between a group of friends with no private data. After initial design discussions, I decided to create a very simple user implementation that does not require passwords for login. It's thus trivial for any user to check or update another user's information, which matches the intent of the site.

Has-Watched List - Once logged in, a user can mark each movie they've watched. They can then see the number of movies they've ever watched, or filter to see the information for each of those movies.

Want-To-Watch List - Similar to the above feature, but used for movies you want to watch in the future. This allows me to find movies multiple people want to see when picking a movie for movie night.

Movie Rating - Users are able to rate movies and compare to the ratings from other users.

Collage - The site can generate one massive collage of all movie posters. Eventually I plan to add the ability to generate mosaics from movie posters. Example image:

## Local Development
cd src/ui

npm install --legacy-peer-deps // installs dependencies

npm run start
