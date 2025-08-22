# AirBnB Clone Project

This is a full-stack clone of the AirBnB platform. The goal is to build a functional web application where users can browse property listings, view details, and complete bookings.

## Project Goals
- Learn to implement responsive UI/UX designs
- Understand how to structure a complex web application
- Gain experience in team collaboration and defined roles
- Practice component-based frontend architecture
- Apply best practices in web application development

## Tech Stack
- **Frontend:** React, HTML, CSS, JavaScript
- **Backend:** Node.js with Express or Django REST Framework
- **Database:** PostgreSQL
- **Version Control:** Git and GitHub
- **Design:** Figma for UI/UX
- **Deployment:** Docker, CI/CD (GitHub Actions)

---

## UI/UX Design Planning

### Design Goals
- Create an intuitive booking flow that minimizes steps for the user.  
- Maintain visual consistency across all pages.  
- Ensure fast loading times and optimized performance.  
- Prioritize mobile-first responsiveness.  

### Key Features
- Property search with filtering and sorting options.  
- Detailed property view with images, amenities, and booking options.  
- Secure and simple checkout process.  
- User authentication for bookings and favorites.  

### Primary Pages

| Page                   | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| **Property Listing View** | Grid display of available properties with search, filters, and sorting options. |
| **Listing Detailed View** | Full property details including photos, amenities, reviews, and booking form.   |
| **Simple Checkout View**  | Streamlined checkout page with price summary, payment form, and confirmation.  |

### Color Styles (from Figma)
- **Primary:** `#FF5A5F`  
- **Secondary:** `#008489`  
- **Background:** `#FFFFFF`  
- **Text:** `#222222`  
- **Secondary Text:** `#717171`  

### Typography (from Figma)
- **Primary Font:** Circular  
- **Headings:** Bold (700), 24px–32px  
- **Body Text:** Medium (500), 16px  
- **Secondary Text:** Book (400), 14px  

### Importance of Identifying Design Properties
Understanding design properties such as colors, typography, and layout choices ensures consistency across the entire application. By clearly defining these elements from the start, the development team can maintain a unified look and feel. It also reduces ambiguity, speeds up collaboration between designers and developers, and helps create a professional, user-friendly product that aligns with user expectations.

---

## Project Roles and Responsibilities

### Project Manager
- Oversees the project timeline and deliverables.  
- Coordinates tasks and ensures smooth collaboration between team members.  
- Tracks progress and resolves scheduling conflicts.  

### Frontend Developers
- Implement the UI components based on Figma designs.  
- Ensure responsive and accessible layouts.  
- Connect frontend with backend APIs.  

### Backend Developers
- Design and implement RESTful APIs.  
- Manage database schema, models, and queries.  
- Implement authentication, booking, and payment logic.  

### Designers
- Create mockups, prototypes, and maintain the design system.  
- Ensure visual consistency and adherence to branding.  
- Provide developers with design assets and specifications.  

### QA/Testers
- Write test cases for functionality and user flows.  
- Perform unit, integration, and end-to-end testing.  
- Report and track bugs for resolution.  

### DevOps Engineers
- Set up and maintain CI/CD pipelines.  
- Manage deployment, environments, and server infrastructure.  
- Monitor application performance and uptime.  

### Product Owner
- Defines project requirements and priorities.  
- Represents the stakeholders and end-users.  
- Validates features and ensures the product aligns with the vision.  

### Scrum Master
- Facilitates agile processes (standups, sprint planning, retrospectives).  
- Removes blockers and ensures smooth team collaboration.  
- Helps the team follow agile best practices.  

---

## UI Component Patterns

To maintain a consistent and reusable interface, the project will define common UI components. These will be built as modular pieces so they can be reused across multiple pages.

### Planned Components

**Navbar**
- Displays the site logo.  
- Includes a search bar for quick property lookups.  
- Provides navigation links (Home, Trips, Favorites, Profile).  
- Features a responsive mobile menu.  

**Property Card**
- Displays a property image.  
- Shows key details: price per night, location, rating.  
- Includes a "favorite" button for saving properties.  
- Designed to adapt to grid layouts on desktop and mobile.  

**Footer**
- Displays links to site pages and policies.  
