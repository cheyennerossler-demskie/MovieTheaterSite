2/24-3/2/2026

- Reviewed Midterm presentation requirements:
  - Timeline of project
  - Discuss working with a team at my internship
  - Knowledge of tech stack
  - Use cases of the software
  - Highlight a feature completed so far this semester
    
## Meeting Notes
Met with Eric on Tuesday 2/24/26 & Friday 2/27/26
- We are utilizing the previously created mapping logic of movie ratings and our MPA-inspired system, based on age, to limit movie results for browse page and specific users
   - New table was introducted to the database schema: UserSettings
       - Ex. UserID: 1 UserSetting: “AgeRestriction“ SettingValue: “6” > This will be read by the system and used to ensure UserID 1 can only see all movies with an MPARatingID under 6
   - When adding a new movie, we should force the rating to be one which already exists in the mapping
- Next to handle: Currently, all types of movies populate up on browse page and are clickable, but when a movie outside of age range is selected, a pop-up says “Error loading movie,” while accepted movies load the movie card pop-up as expected
  - Instead, restricted results need to be removed from display entirely

### Commits > Frontend:
- Fixed navigation of browser's back/forward buttons
  - Tested relevant pathways, all were successful
- Updated link for Rotten Tomatoes ratings on movie card pop-ups

### Commits > Backend:
- Leveraged UserSettings table to help filter pages based on mapped age restrictions
  - HotChocolate GQL query extension created
- Added authentication cookies to access user's ID when logging in, persists for 30 days
