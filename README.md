# Movie Theater Site
Senior Project, SUNY New Paltz
Spring 2026

## Link to Project
![Flatbox Studios logo](pics/flatbox.png)

https://github.com/ecarpouzis/MovieTheater.git
- Flatbox Studios Supervisor: Eric Carpouzis

## Overview
Movie Theater Site is a web-application to celebrate cinema and combat the endless options of films available throughout the streaming-service world. This site tracks watched movies, want-to-watch movies, and personalized movie ratings to assist with planning movie nights! 

![Movie Site](pics/moviesite.png)

# Features
- Users
    - Discover friend’s lists
    
- Movies & Actors
    - Search capabilities

- Watched 
    - Once logged in, a user can mark each movie they've watched and they can then see the number of movies they've ever watched, or filter to see the information for each of those movies

- Want-To-Watch Lists	
    - Similar to the above feature, but used for movies you want to watch in the future

- Ratings
    - Users are able to rate movies and compare to the ratings from other users

- Posters
    - The site can generate one massive collage of all movie posters

![Movie collage](pics/moviecollage.png)

### Future Features:
- Request movies to add to site 
- Trailers for movies
- Streaming services available per movie
- Generate mosaics from movie posters

## Collection References
- 1001 Movies To Watch Before You Die
- National Film Registry (Library of Congress)
- The Criterion Collection

## Tech Stack
Movie Theater Site is an open-source .NET 8 CRUD entity-management application leveraging open APIs, such as Google’s Programmable Search Engine API, with a front-end driven by React.

Movie Data & Posters 
- Data has been retrieved through various methods including web scraping and API access
- Posters were once stored as BLOBs, but now stored as files because it’s faster and less resource-intensive
- When a new movie is added to the site, a Python script is run to create a high quality/small sized thumbnail, which is used when browsing for movies
Users 
- A typical ASP.Net Identity implementation would be trivial, but this site is communally shared between Flatbox Studio members and friends, with no private data

### Lanaguages & Frameworks
- Backend: **C#** & **Python**
    - Visual Studio 

- Frontend: **React**, **HTML**, & **CSS** 
    - Visual Studio Code

- Database: **GQL**
    - SQL Server Management Studio

- Containerization: **Docker** & **Kubernetes** 

## Local Development
### Clone GitHub Repository: https://github.com/ecarpouzis/MovieTheater.git

Run commands in terminal:

**cd src/ui**

**npm install --legacy-peer-deps** // installs dependencies

**npm run start**

- React runs on localhost:3000, C# runs on localhost:3001
