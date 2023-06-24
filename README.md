# VPN Web Application
This is a web application designed for managing VPN services provided by a VPN service provider company. The application allows administrators to register, add service providers, and associate countries with the service providers. Users can register themselves, subscribe to a service provider, and connect to a VPN service in a specific country. Users can also communicate with each other, provided they are in the same country or connected to a VPN in the same country.

## High-Level Requirements
The following are the key requirements of the VPN web application:

- Administrators can:
  - Register themselves using the registerAdmin endpoint.
  - Add service providers using the addServiceProvider endpoint.
  - Add countries to the service providers using the addCountry endpoint.

- Users can:
  - Register themselves using the registerUser endpoint.
  - Subscribe to a service provider using the subscribe endpoint.
  - Connect to a VPN service in a specific country using the connect endpoint.
  - Disconnect from the VPN using the disconnect endpoint.
  - Establish communication with other users using the communicate endpoint.
    
## API Endpoints
The VPN web application uses a RESTful API approach with the following controllers and endpoints:

### AdminController
- `/register` - POST request to register a new administrator.
- `/addProvider` - POST request to add a new service provider.
- `/addCountry` - POST request to add a country to a service provider.
### UserController
- `/register` - POST request to register a new user.
- `/subscribe` - PUT request to subscribe a user to a service provider.
### ConnectionController
- `/connect` - POST request to connect a user to a VPN service in a specific country.
- `/disconnect` - DELETE request to disconnect a user from the VPN.
- `/communicate` - GET request to establish communication between users.
## Models
The web application uses the following models:

* `Admin` : Represents an administrator.
* `User` : Represents a user who can subscribe to a service provider and connect to VPN services.
* `ServiceProvider` : Represents a service provider that offers VPN services.
* `Country` : Represents a country to which VPN services can be connected.
* `Connection` : Represents a connection between user and service provider. 
## Technologies Used
The VPN web application is built using the following technologies:

* **Java**
* **Spring Boot**
* **Spring Data JPA**
* **RESTful APIs**
## Setup and Installation
To set up the VPN web application locally, follow these steps:

1. Clone the repository from GitHub.
2. Open the project in your preferred IDE.
3. Build the project to resolve dependencies.
4. Configure the application properties with your database connection details.
5. Run the application.
6. Access the API endpoints using a tool like **Postman** or **Swagger-UI**.
## Contributions
Contributions to the VPN web application are welcome! If you encounter any issues or have suggestions for improvement, please create a new issue or submit a pull request.
