2/3-9/2026

## Meeting Notes
Met with Eric on Tuesday 2/3/26
- Reviewed initial tasks put on a "To Do" board in Jira
    - We will identify and update each task's priority 
    - I will create pull requests (PR) per task and Eric will review before committing to main branch
- Was given access to database 
    - Reminded to 'ignore' details such as database password, keys, etc. > don't commit to GitHub
    - Discussed SimpleTitle vs. Title columns in Database
    - Collection of movies dervied from various "best of" lists ex. 1001 Movies to Watch Before You Die, National Film Registry (Library of Congress), etc.
- Verified local development setup:
cd src/ui
npm install --legacy-peer-deps // installs dependencies
npm run start

Suggestions: 
- Copilot account
- Playwright / Selenium (automation)

## Current tickets:
- Movie Panel 2.0 
    - Open a pop-up for a chosen movie instead of changing pages
- Enable automatic table backups 
    - When a db insert takes place, it would be good to run a script that checks if we have a backup from that day, takes a backup if we do not have one, deletes backups older than a certain timeframe, and store details about backups 
- Batch Insert doesn't refresh the style of elements when a new batch is generated 
    - Currently after a movie is inserted, the insert button changes color to indicate we’ve inserted it. If we then generate another batch, the color change stays
- Image Caching Cache
    - Image Caching is slow and scrolling through letters quickly reveals the issue. Not sure if we can proactively cache or what other strategies we can leverage, we already have a python script creating thumbnails of posters for navigation purposes
-Site Navigation Pass 
    - Clicking letters for searching, searching for a movie, search for an actor by name, insert or edit a movie
- Edit Movie Functionality > part 2 of Movie Panel 2.0
- Edit Poster Functionality > part 2 of Edit Movie Functionality
- Poster Max Height/Width 
    - Consistency of image sizes, create new component for display

## Agile Methodology
- Jira ticket board:
![Jira boarc](Jiraboard.png)


