# Real Estate Management System

A comprehensive Java-based web application for managing real estate properties with an efficient Binary Search Tree (BST) implementation for property organization and retrieval.

## 📋 Description

This Real Estate Management System is a university project that demonstrates advanced data structures and web development concepts. The system uses a custom Binary Search Tree to efficiently manage and search properties based on price, providing optimal performance for property listings and queries.

## ✨ Key Features

### Core Functionality
- **Binary Search Tree Implementation**: Custom BST for efficient property sorting and searching by price
- **Role-Based Access Control**: Three distinct user roles with specific permissions
  - **Admin**: Full system control, user management, property oversight
  - **Seller**: Create, edit, and manage property listings
  - **Buyer**: Browse properties, add to favorites, submit feedback

### Property Management
- **CRUD Operations**: Complete Create, Read, Update, Delete functionality for properties
- **Advanced Search & Filter**: Search by location, price range, property type, bedrooms, bathrooms
- **Image Upload**: Multi-image support for property listings
- **Property Details**: Comprehensive property information including area, type, and amenities

### User Features
- **User Registration & Authentication**: Secure login/logout with session management
- **Profile Management**: Edit user profiles and account settings
- **Favorites/Wishlist**: Buyers can save and manage favorite properties
- **Feedback System**: Submit, view, and manage property reviews and ratings

### Admin Features
- **User Management**: View, create, and delete user accounts
- **Property Oversight**: Manage all property listings across the platform
- **Admin Creation**: Add new administrators to the system
- **Feedback Moderation**: View and manage user feedback

## 🛠️ Technology Stack

### Backend
- **Java 22**: Latest Java version for modern features
- **Java Servlets 4.0**: Request handling and business logic
- **JSP 2.3**: Dynamic web page generation
- **Maven**: Dependency management and build automation

### Frontend
- **HTML5/CSS3**: Responsive user interface
- **JavaScript**: Client-side interactivity and form validation
- **JSTL 1.2**: JSP Standard Tag Library for cleaner JSP pages

### Libraries & Dependencies
- **Gson 2.10.1**: JSON serialization/deserialization
- **JUnit 4.13.2**: Unit testing framework
- **Servlet API 4.0.1**: Web application framework
- **JSP API 2.3.3**: JavaServer Pages support

### Data Management
- **File-Based Storage**: JSON files for data persistence
- **Custom Data Structures**: Binary Search Tree for optimized property management

### Architecture
- **MVC Pattern**: Model-View-Controller design pattern
- **Service Layer**: Separation of business logic
- **Utility Classes**: Reusable components for file management and constants

## 📁 Project Structure

```
New_Finalized/
├── src/
│   ├── main/
│   │   ├── java/com/realestate/
│   │   │   ├── model/              # Data models
│   │   │   │   ├── Admin.java
│   │   │   │   ├── Buyer.java
│   │   │   │   ├── Seller.java
│   │   │   │   ├── Property.java
│   │   │   │   ├── Feedback.java
│   │   │   │   └── User.java
│   │   │   ├── service/            # Business logic
│   │   │   │   ├── UserService.java
│   │   │   │   ├── PropertyService.java
│   │   │   │   └── FeedbackService.java
│   │   │   ├── servlet/            # Request handlers
│   │   │   │   ├── LoginServlet.java
│   │   │   │   ├── RegisterServlet.java
│   │   │   │   ├── PropertyServlet.java
│   │   │   │   ├── AdminServlet.java
│   │   │   │   ├── FeedbackServlet.java
│   │   │   │   └── UserServlet.java
│   │   │   └── util/               # Utility classes
│   │   │       ├── PropertyBST.java     # Binary Search Tree
│   │   │       ├── FileUtil.java        # File operations
│   │   │       ├── FileManager.java
│   │   │       └── Constants.java
│   │   └── webapp/
│   │       ├── WEB-INF/
│   │       │   └── web.xml         # Servlet configuration
│   │       ├── css/                # Stylesheets
│   │       ├── js/                 # JavaScript files
│   │       ├── images/             # Static images
│   │       ├── data/               # Data storage files
│   │       └── *.jsp               # JSP pages
│   └── test/                       # Unit tests
├── pom.xml                         # Maven configuration
└── README.md
```

## 🚀 Installation & Setup

### Prerequisites
- **Java Development Kit (JDK) 22** or higher
- **Apache Tomcat 9.0+** or any compatible servlet container
- **Maven 3.6+** for dependency management
- **IDE** (IntelliJ IDEA, Eclipse, or NetBeans recommended)

### Setup Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/realestate-management-system.git
   cd realestate-management-system
   ```

2. **Build the Project**
   ```bash
   mvn clean install
   ```

3. **Configure Data Paths**
   - Update file paths in `FeedbackService.java` and other service classes to match your local directory structure
   - Default data storage location: `src/main/webapp/data/`

4. **Deploy to Tomcat**
   - Copy the generated WAR file from `target/real-estate-management.war` to Tomcat's `webapps` directory
   - Or configure your IDE to deploy directly to Tomcat

5. **Start the Server**
   - Start Apache Tomcat server
   - Access the application at: `http://localhost:8080/real-estate-management/`

6. **Default Admin Access**
   - Create an admin account through the admin registration page
   - Navigate to `/add-admin.jsp` (may require initial setup)

## 📖 Usage Guide

### For Buyers
1. **Register** a new buyer account
2. **Browse** available properties on the property listing page
3. **Search** properties by location, price, or features
4. **View Details** of individual properties
5. **Add to Favorites** to save properties for later
6. **Submit Feedback** on properties you've viewed

### For Sellers
1. **Register** as a seller
2. **Add New Properties** with details and images
3. **Manage Listings** - edit or remove your properties
4. **View** all your active listings

### For Administrators
1. **Login** with admin credentials
2. **Manage Users** - view, create, or delete accounts
3. **Oversee Properties** - manage all property listings
4. **Review Feedback** - monitor user feedback
5. **Create Admins** - add new administrators

## 👨‍💻 Author

**Your Name**
- GitHub: https://github.com/yasithsenarathyapa
- Email: yasithsenarathyapa.info@gmail.com

## 🙏 Acknowledgments

- University coursework project
- Implements core data structures and algorithms concepts
- Demonstrates MVC architecture in Java web applications

## 📞 Support

For any queries or issues, please open an issue on GitHub or contact the developer.
