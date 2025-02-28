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





-------
-----
---
---


## **Day 6 Report**  

### **Tasks Completed**  

1. **Converted Vite Project to Next.js**  
   - Successfully migrated the **home page** from Vite to Next.js.  
   - Refactored components to follow Next.js structure, including **App Router** and **dynamic routing**.  
   - Ensured smooth integration with **server-side rendering (SSR) and static site generation (SSG)**.  

2. **Fixed Asset Import Issues**  
   - Resolved the `Module not found: Can't resolve '../assets/images/logo.png'` error by properly handling image imports in Next.js.  
   - Used `public/` directory for static assets like `icon.png`.  

3. **Installed and Configured Tailwind CSS**  
   - Successfully integrated **Tailwind CSS** into the Next.js project.  
   - Configured `tailwind.config.js` to ensure proper **content scanning** for class usage.  

4. **Metadata & Icon Setup**  
   - Added proper metadata for `internee.pk`, including **title and description**.  
   - Integrated a **favicon (`icon.png`)** for branding consistency.  

5. **Fixed Missing Dependencies**  
   - Installed **react-multi-carousel** and resolved `Module not found: Can't resolve 'react-multi-carousel'` error.  
   - Ensured all necessary dependencies were properly added to `package.json`.  

---

### **Challenges**  
- Handling **image imports** correctly, since Next.js uses `public/` for static assets.  
- Adjusting Tailwind CSS configurations to work efficiently in a Next.js environment.  

---

### **Next Steps**  
1. **Complete Full Page Migration**  
   - Convert remaining pages and components from Vite to Next.js.  
   - Ensure proper handling of **dynamic routing and API calls**.  

2. **Further Optimization**  
   - Optimize page load performance with **lazy loading** and **image optimization**.  
   - Improve SEO with **structured metadata and Open Graph tags**.  

3. **Enhance UI/UX**  
   - Refine the **responsive design** using Tailwind.  
   - Ensure accessibility best practices are followed.  

-------
-----
---
---


## **Day 7 Report**  

### **Tasks Completed**  

1. **Set Up Internship Schema in Database**  
   - Configured and structured the **internship schema** in the database using Drizzle and PostgreSQL.  
   - Ensured **relationships and indexing** for efficient querying.  

2. **Rendered Internship Categories from Database**  
   - Successfully fetched **categories dynamically** from the database.  
   - Implemented efficient data fetching strategies with **server-side rendering (SSR)** in Next.js.  

3. **Enhanced UI and Animations for Internship Page**  
   - Improved the **premium look and feel** of the internship page.  
   - Implemented **scroll-based animations** with Framer Motion to load cards one by one as the user scrolls.  
   - Added **hover effects** and smooth transitions for an interactive user experience.  

4. **Fixed Data Fetching Issues**  
   - Debugged and resolved **async issues** in fetching subcategories.  
   - Ensured proper **error handling** and data validation before rendering components.  

5. **Optimized Grid Layout for Internship Categories**  
   - Implemented a **responsive grid** using Tailwind CSS.  
   - Ensured a seamless experience across different screen sizes, from **mobile to desktop**.  

---

### **Challenges**  
- Handling **async data fetching** efficiently while keeping the UI responsive.  
- Ensuring **Framer Motion animations** worked smoothly in Next.js **App Router**.  
- Adjusting **grid responsiveness** for a balanced design.  

---

### **Next Steps**  
1. **Complete Internship Detail Page**  
   - Implement **dynamic routing** to show internship details.  
   - Optimize content structure for better readability.  

2. **Improve Performance**  
   - Optimize **database queries** for faster data retrieval.  
   - Implement **lazy loading** for assets and images.  

3. **Enhance Search & Filter Functionality**  
   - Add a **search bar** and category-based filters for better UX.  
   - Ensure smooth filtering without excessive re-renders.  


