# AirBnB Clone Project
The Airbnb Clone Project is a full-stack web application that simulates the core features of the Airbnb platform. It is designed to provide hands-on experience in building scalable, secure, and feature-rich booking systems while following industry best practices. The application allows users to browse property listings, view detailed information, and complete bookings, offering a functional and realistic clone of the Airbnb platform.

## Project Goals Front End
- Learn to implement responsive UI/UX designs
- Understand how to structure a complex web application
- Gain experience in team collaboration and defined roles
- Practice component-based frontend architecture
- Apply best practices in web application development
## Project Goals BackEnd
-Build a robust backend system to handle bookings, users, properties, and reviews.
-Design a relational database that models real-world requirements.
-Develop secure APIs with authentication and authorization.
-Create a responsive frontend interface that ensures a smooth user experience.
-Implement CI/CD pipelines for streamlined deployment.
-Foster collaborative team workflows through GitHub-based project management.


## Tech Stack
- **Frontend:** React.js (with Tailwind CSS for styling)
- **Backend:** Node.js with Express or Django REST Framework
- **Database:** PostgreSQL,MySQL
- **Version Control:** Git and GitHub
-**API:** REST and GraphQL
- **Design:** Figma for UI/UX
- **Deployment:** Docker, CI/CD (GitHub Actions)

## Technology Stack

- **Frontend:** React.js (with Tailwind CSS for styling)
- **Backend:** Node.js with Express or Django REST Framework
- **Database:** PostgreSQL,MySQL
- **Version Control:** Git and GitHub
-**API:** REST and GraphQL
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

## Team Roles and Responsibilities

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

### Database Administrator (DBA)

-Designs, manages, and optimizes the database. 
-Ensures data integrity, availability, and security.

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

### Database Design
**Key Entities and Fields**

**1. Users**
-id (primary key)
-name
-email
-password
-role (guest or host)

**2. Properties**
-id (primary key)
-user_id (foreign key to Users)
-title
-description
-location
-price_per_night

**3. Bookings**
-id (primary key)
-user_id (foreign key to Users)
-property_id (foreign key to Properties)
-check_in_date
-check_out_date
-status (pending, confirmed, cancelled)

**4. Reviews**
-id (primary key)
-user_id (foreign key to Users)
-property_id (foreign key to Properties)
-rating
-comment

**5. Payments**
-id (primary key)
-booking_id (foreign key to Bookings)
-amount
-payment_date
-payment_status (completed, pending, failed)

### Relationships
-A User can own multiple Properties.
-A User can make multiple Bookings.
-A Booking belongs to one Property and one User.
-A Property can have multiple Reviews, each created by a User.
-A Payment is linked to one Booking.

### Feature Breakdown

**1. User Management**
This feature allows users to register, log in, and manage their profiles. It also handles user roles, distinguishing between guests and hosts, ensuring personalized experiences.

**2. Property Management**
Hosts can list properties, add details such as descriptions, pricing, and location, and manage availability. This feature ensures properties are searchable and accessible to potential guests.

**3. Booking System**
Guests can check property availability, create bookings, and track booking status. This feature manages reservations, preventing double bookings and maintaining accurate property schedules.

**4. Review System**
Guests can leave reviews and ratings for properties they have stayed in. This helps build trust, improves transparency, and provides feedback for hosts.

**5. Payment Processing**
This feature manages payments for bookings, handling amounts, payment statuses, and transaction history. It ensures secure processing and tracks payment confirmations.

**6. Search and Filter**
Guests can search properties based on location, price, availability, and other filters. This feature enhances usability and improves the guest’s ability to find suitable options quickly.