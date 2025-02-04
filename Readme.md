# Day 1 Report

## Summary
- Understood the Drizzle ORM, focusing on the creation of a new schema for storing user badges.
- Created the **Badges** schema to track the badges awarded to users.
  
## Tasks Completed
- Created a new schema for badges, where each user can have multiple badges linked to them.
- Set up the necessary fields in the schema, including:
  - Badge name
  - User ID
  - Date awarded
  - Criteria for badge assignment
  
- Developed an API endpoint to create and assign badges to users.

## Challenges Faced
- Minor challenges with schema structure adjustments for scalability.
  
## Next Steps
- Plan to work on the badge creation logic triggered by interview performance. The badge will be awarded when an interview score exceeds 7.

-------
-----
---
---

# Day 2 Report

## Summary
- Rendered badge data on `badges/page.jsx` with a clean UI.
- Added a loading screen for better UX during data fetch.
- Implemented a sidebar for improved navigation.

## Tasks Completed
1. **Rendered Badge Data**:
   - Fetched and displayed badge data (names, descriptions, dates) on `badges/page.jsx`.

2. **Loading Screen**:
   - Added a skeleton loader for smoother data fetching.

3. **Sidebar**:
   - Created a sidebar for easier app navigation.

4. **Dynamic Routing**:
   - Started migrating to `badges/[userid]/page.jsx` for user-specific badge pages.

## Challenges
- Ensuring responsive and consistent UI across devices.
- Managing loading states without layout shifts.

## Next Steps
1. **Badge Assignment Logic**:
   - **Golden Badge**: Score > 9 in an interview.
   - **Silver Badge**: Score > 7 in an interview.

2. **Dynamic User Badge Pages**:
   - Complete migration to `badges/[userid]/page.jsx` for unique user URLs.

3. **Shareable Badges**:
   - Enable users to share badge pages on social media or via links.