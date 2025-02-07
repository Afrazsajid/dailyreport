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
- Plan to Render the badges on screen with handling loading problems.

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



-------
-----
---
---

# Day 3 Report

## Summary
- Designed a schema for badge overrating based on MOCI interview scores to trigger badge assignments.
- Made the feedback page dynamic to display overrating.
- Enabled users to share their badge pages to showcase achievements.
- Started working on a more scalable approach to badge assignment.

## Tasks Completed
1. **Badge Overrating Schema**:
   - Created a schema for triggering badges based on interview performance (MOCI).
   - Focused on score thresholds to assign badges like **Golden** (score > 9) and **Silver** (score > 7).

2. **Dynamic Feedback Page**:
   - Updated the feedback page to dynamically display overrating information, reflecting the badge scores.

3. **Badge Criteria Schema**:
   - Designed a scalable badge criteria schema, factoring in interview counts and badge quantities.
   - Created a logic flow diagram to guide the dynamic assignment of badges without bloating code for each new badge type.

4. **Shareable Badges Page**:
   - Implemented the functionality to make badge pages shareable, allowing users to share their achievements via links or social media.

## Challenges
- Creating a scalable badge assignment system that can handle an increasing number of badges.
- Determining an efficient way to reduce load as the number of badges grows, preventing excessive logic functions for each new badge.

## Next Steps
1. **Badge Assignment Logic**:
   - Implement the badge assignment logic using the schema to efficiently assign badges based on interview performance and counts.
   - Consider using a combined "King" badge for top rankers when there are multiple high-performing candidates.

2. **Optimizing Badge Assignment**:
   - Refine the badge assignment system to reduce logic redundancy and optimize performance as more badge types are added.



-------
-----
---
---



## **Day 4 Report**  

### **Tasks Completed**  
1. **Badge Assignment Logic Implemented**  
   - Successfully implemented the logic to assign **Golden** and **Silver** badges based on interview scores.  
   - Ensured that badge assignment is dynamic, using the previously designed schema.  

2. **Performance Optimization in Badge Assignment**  
   - Refactored the logic to improve efficiency and prevent redundant function calls.  
   - Structured the system to scale as more badge types are introduced.  

### **Challenges**  
- Ensuring the badge assignment remains scalable and efficient, especially as more badges are introduced.  
- Preventing performance bottlenecks while checking badge eligibility dynamically.  

### **Next Steps**  
1. **Implement "Big Badge" System**  
   - Assign users a special badge (e.g., **Elite Badge**) when they collect three **Golden** or **Silver** badges.  
   - Ensure smooth integration into the current badge assignment logic.  

2. **Further Optimization**  
   - Fine-tune the badge assignment process to handle edge cases efficiently.  
   - Continue refining the logic to prevent unnecessary database queries and function calls.  




