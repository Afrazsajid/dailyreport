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





 # Day 3 Report

## Summary
- Designed a schema for overrating in the MOCI interview to trigger badges.
- Made the feedback page dynamic to display overrating data.
- Explored a scalable badge assignment method to handle future badge additions efficiently.

## Tasks Completed
1. **Overrating Schema Implementation**:
   - Created a schema to capture overrating in the MOCI interview.
   - Integrated logic to trigger badges based on overrating.

2. **Dynamic Feedback Page**:
   - Modified the feedback page to dynamically display overrating details.

3. **Badge Assignment Challenge**:
   - Encountered an issue where manually assigning badges through separate functions per badge type would not scale well.
   - Identified that adding more badge types would lead to increased function complexity and system load.

4. **Scalable Badge Assignment Plan**:
   - Proposed creating a **badge criteria schema** to dynamically determine badge assignments.
   - Designed three badge categories based on:
     1. Number of interviews completed.
     2. Number of badges earned.
     3. Top rankers (e.g., if there are 3 top rankers, assign a "King" badge to them).
   - Spent time creating a logic flow diagram to optimize badge assignment.

## Challenges
- Finding an efficient method to check and assign a large number of badges without increasing system load.
- Ensuring badge assignment remains flexible as more badge types are introduced.

## Next Steps
1. **Implement Badge Criteria Schema**:
   - Develop a schema to handle badge logic dynamically instead of hardcoding badge assignments.

2. **Optimize Badge Assignment Logic**:
   - Implement an efficient query mechanism to determine badge eligibility without excessive function calls.

3. **Complete Badge Assignment Integration**:
   - Finalize and test the logic to assign badges based on the new schema.

4. **Refine Feedback Page**:
   - Ensure overrating details are properly integrated and visually clear for users.

5. **Prepare for Shareable Badges**:
   - Start planning how users can share their earned badges through social media or direct links.

