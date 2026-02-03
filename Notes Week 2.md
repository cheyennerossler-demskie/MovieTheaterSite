1/27-2/2/2026

## Meeting Notes
Met with Eric on Tuesday 1/26/26
- Verified Install: Visual Studio 2026, Visual Studio Code 
- Installed: SQL Service Management Studio (Database)

- Visual Studio > C# (functionality) > Reason for using it:
    - ASP .NET 
    - Data binding / data types vs. Node.js JavaScript 
    - Accessible with Linus / Mac
- Visual Studio Code > frontend

- Single page app 
- Goal: see “Friends icons” for seen/want/ratings
- Goal: Ui / React > pop-ups vs. new page
- Version Control app:  Jira

## Current tasks ideas:
1. Ability to edit an entity
2. Ability to re-download and re-shrink a Poster
3. Release Date parsing is still pretty rigid, can't do something like 'November 13 2018'
4. Need to fix insert logic. Thelma becomes "ma, The"
5. Set a max height/width on all poster displays
6. Batchinsert doesn't play nice without page refreshing (at least the styling of insert buttons is wrong)
7. Batchinsert doesn't play nice with clicking to other pages, not a true Single Page Application
8. Clicking a movie should display the movie in a popup rather than take over the full display
9. Smarter/Dynamic collage (check if the collage functionality still works)
10. Clicking one letter into another should deselect old selection
11. Some movies don't use real IMDB IDs, this should be marked in some way to prepare for data processing
12. Use my IMDB IDs to fill more actors, better actor handing & styling
- Above, but with movie summaries
- Above, but with RT/IMDB ratings
13. Fix ratings would be nice
14. Suggest-a-movie feature (currently everything is me setting something as 'Want to Watch' for someone)
15. Request-a-movie feature (enter in an IMDB ID, I know to go and find that movie)
16. Ratings filter, explicit flag I think exists for 'WILL NOT SORT' but I need a way to prevent some movies from showing up for anyone other than users marked 
17. More ways to filter movies and watchlists (Show me G/PG rated movies on Alex's list)
18. Automatic table backups to prevent me from accidentally wiping out a field when doing a SQL update
19. Mobile support (current display looks very bad on mobile)
20. Cleanup old users
21. Review Thumbnail logic, ensure syncing to and from local dev is reasonable
22. Fix syncing with our remote file backup
23. My small application that creates a directory list text file includes itself and should not
24. Improvements to folder generation logic
25. Improvements to insert->doc update->file insert workflow
26. Logic to check missing/incorrect movies, empty folders

===Hard but cool===
1. Mosaic generation
2. AI movie suggestions, especially once I have ratings in
3. Track file location of movies would be great, click-through to movie would be nice. Jellyfin Stream is a pipedream
4. Letting the site begin/drive channels on devices

## MY ideas for site:
- Make size of window dynamic > Alphabet / Scroll bar
- Better loading screen > Searching
- Better results descriptions > Number / List / Sort / Filter
    - Ex. Begins with / Contains / Ends with 
- Multiple search selects > Filters
    - Ex. Movie Title & Actor Name > Specify first / last name, etc. 
- Back to previous page / “homepage” from search/selection > Goes to “batchinsert”
- Needs “Menu” options
- “Username” shouldn’t show ALL usernames > only per user  
- “Friends” menu > can’t login nor change their selections
- Seen vs. Want under username > “65” / “38” (these reflect the # in each group)
- When clicked, return to top of page
- Another option: “Want to Rewatch”
- When a Seen / Want is updated, refresh the page?
- Ratings for each entry
