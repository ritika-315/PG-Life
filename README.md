PG Life - README
Introduction
PG Life is a web application that helps users find and explore Paying Guest (PG) accommodations in various cities. The platform offers a comprehensive listing of properties, complete with detailed information, ratings, and user interest levels. Users can search for properties, filter results based on gender preferences, and sort listings by rent. The application also features user authentication, allowing interested users to mark properties they like.

Features
City-Based Property Listings
PG Life allows users to view PG properties based on their chosen city. By selecting a city from the list, users can see a curated list of PG accommodations available in that city. The city details are fetched from the database, ensuring up-to-date information.

Search Functionality
Users can search for specific properties within a city using the search bar. This feature enables users to quickly find properties that match their criteria by searching for property names.

Sorting and Filtering
To enhance the user experience, PG Life provides sorting and filtering options:

Sorting: Users can sort properties by rent in ascending or descending order, allowing them to find accommodations within their budget.
Filtering: Users can filter properties based on gender preferences (male, female, unisex), ensuring they find suitable accommodations that meet their needs.
Property Details
Each property listing includes:

Images: A visual representation of the property.
Ratings: Cleanliness, food quality, and safety ratings are aggregated to provide an overall rating.
Interested Users: A count of users interested in the property, with a visual indicator if the current user has shown interest.
User Authentication and Interest Tracking
Authenticated users can express interest in properties, which is tracked and displayed on the property listings. This feature helps users keep track of properties they like and see how many others are interested in the same properties.

Mobile-Friendly Design
The application is designed to be responsive, ensuring a seamless experience across various devices. Bootstrap's grid system and utility classes are utilized to enhance mobile friendliness without altering the original code structure.

Code Overview
Backend (PHP and MySQL)
The backend is implemented in PHP, connecting to a MySQL database. Key functionalities include:

Session Management: Handling user sessions for authentication.
Database Connections: Fetching city and property details from the database.
Search, Sort, and Filter Logic: Building SQL queries based on user inputs to retrieve relevant property listings.
Frontend (HTML, CSS, and JavaScript)
The frontend uses a combination of HTML, CSS, and JavaScript (including jQuery and Bootstrap) to provide an interactive and user-friendly interface. Key components include:

Header and Footer: Included across all pages for consistent navigation and branding.
Property Listings: Dynamically generated based on database queries, with responsive design enhancements.
Modals: Used for filters and user authentication forms.
Styles and Responsiveness
Custom CSS is used alongside Bootstrap to ensure the application looks good on all devices. Specific styles are added to make property cards, search bars, and filter options adapt to different screen sizes.

Getting Started
Prerequisites
Web Server: Apache or Nginx.
PHP: Version 7.0 or higher.
MySQL: Version 5.6 or higher.
Composer: For managing PHP dependencies.
Installation
Clone the Repository:
git clone https://github.com/yourusername/pglife.git
Navigate to the Project Directory:
cd pglife
Install Dependencies:
composer install
Set Up the Database:
Create a new phpMyAdmin database.
Import the provided SQL script to set up the necessary tables.
Configure the Application:
Update the includes/database_connect.php file with your database credentials.
Ensure the server settings are correctly configured in includes/config.php.
Running the Application
Start the Web Server:
For Apache, ensure the httpd service is running.
For Nginx, ensure the nginx service is running.
Access the Application:
First start the Apache and MySql in xammp controller then ->
Open your web browser and navigate to http://127.0.0.1/PGLife/.
Conclusion
PG Life is a robust platform designed to simplify the process of finding PG accommodations. With features like city-based listings, search, sort, and filter options, and user interest tracking, the application aims to provide a comprehensive solution for users looking for PG accommodations. The mobile-friendly design ensures that users can access the platform seamlessly from any device.
