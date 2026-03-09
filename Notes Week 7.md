3/3-3/9/2026

- Learned Hot keys for VS 2022:	
  - Ctrl+T = search for files 
  - Highlight, F12 = find instances of methods, variables, etc.
  - F12 on site = view mobile verison of browser
    
## Meeting Notes
Met with Eric on Wednesday 3/4/26
- We reviewed the functionality of the new rating mappings
  - We've decided to leave the browse page as a random selection of 50 movies including all types of ratings
  - Cookie authorization has been update to remove UserID when logging out to properly refresh the browse page
- We reviewed how a lot of the current updates are only reflected on the frontend, but, eventually, the backend architecture will be altered to further filter data
- Eric made 2 major updates to help prepare for new mobile version
1. Migration to OData/LINQ > away from Apollo, to run GQL server, and HotChocolate (.NET framework)
  - Reason for this switch:
    - Deep, dynamic queries aren't needed, too complex for dataset
    - doesn't require regeneration or running a server in the site's Docker container
    - Overall simplification of backend
2. Structural UI changes via Vite & React > instead of just React
- Reason for this switch:
  - Version of React previously used is deprecated
  - Industry standard, translates React (HTML/CSS/JSX) files into objects sent to the browser

### Commits > Frontend:
- Updated URLs to a safer scheme
  - We want to hide internal code from public URL
    - Not completed / Not merged
- Added page / search headers
  - Each page should have a heading to describe path of use, helpful when using back/forward buttons
    - Not completed / Not merged

## Midterm Presentation Outline:
- Overview
  - About the application
  - Tech Stack
  - Languages & Frameworks
- Internship
  - Teamwork
    - Version control 
    - Communication
  - Preparedness
    - Planning meetings
    - Ask questions
  - Exposure
    - Ways of working / techniques
    - Technologies
- Timeline
- Features
  - Use cases
  - Highlight > Rating Mappings & Mobile styling
  - Future goals
