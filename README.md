# Blood Bank Application

The **Blood Bank Application** is a comprehensive web application developed to efficiently manage blood donation and distribution processes. With a user-friendly interface and distinct roles, including user, hospital, organization, and admin, the application adapts its functionalities based on the role.

## Features and Functionalities

- **Role-Based Functionalities:** The application offers role-specific features:
  - **User:** Users can donate or consume blood, view related organizations, and track their blood donations to specific organizations.
  - **Hospital:** Hospitals can monitor user and organization blood donation quantities related to their facility.
  - **Organization:** Organizations can view connected hospitals and users along with their donated blood quantities.
  - **Admin:** Admins can manage the application by deleting donors, hospitals, and organizations.

- **Shared Forms:** A single form is used for login and registration across all roles, ensuring a consistent user experience.

- **Real-time Data Retrieval:** Utilizing an Axios interceptor, the application fetches data from the server-side. The interceptor sets a base URL and token for secure and seamless communication.

- **Analytics Page:** Donors, hospitals, and organizations have access to an analytics page showcasing blood type statistics, total blood in, total blood out, available blood for each type, and recent transactions.

## Technology Stack

The project employs the MERN (MongoDB, Express, React, Node.js) stack for its development:

- **MongoDB:** Store and manage data related to users, roles, blood donations, and transactions.

- **Express.js:** Create robust APIs to handle user actions and interactions.

- **React.js:** Build the user interface and user experiences for the application.

- **Node.js:** Develop the backend logic and APIs to support user roles and functionalities.

- **Redux:** Manage the state of the application, enabling efficient data flow between components.

## Getting Started

To use the Blood Bank Application, follow these steps:

1. **Clone or Download:**

   Clone this repository to your local machine using the following command:
  ```git clone https://github.com/gautamkhatik/bb.git```

Alternatively, download the repository as a ZIP file.

2. **Environment Variables:**

In the `api` folder, set environment variables in a `.env` file:
`PORT=<your-port>`
`JWT_SECRET=<your-jwt-secret>`
`MONGO_URL=<your-mongo-url>`

Similarly, in the `client` folder, set the `REACT_APP_BASE_URL` environment variable in a `.env` file:

REACT_APP_BASE_URL=<your-react-base-url>

If you are running the application locally, set the following for the `REACT_APP_BASE_URL`:

`REACT_APP_BASE_URL=http://localhost:8080/api/v1`

3. **Install Dependencies:**

In both the `api` and `client` folders, install required dependencies:
`cd blood-bank-application/api`
`npm install`
`cd blood-bank-application/client`
`npm install`

4. **Run the Application:**

Start the API server and the client application in their respective folders:
```cd blood-bank-application/api```
```npm start```
`cd blood-bank-application/client`
`npm start`

5. **Access the Application:**

Open your web browser and navigate to `http://localhost:3000` to use the application.

## Usage

1. **Login and Registration:**

Utilize the single login and registration form based on your role.

2. **Role-Specific Functionalities:**

Explore functionalities tailored to each user role, including blood donation, blood consumption, organization management, and more.

3. **Analytics Page:**

Access the analytics page to view blood type statistics, total blood in, total blood out, available blood, and recent transactions.

4. **Admin Control:**

Admins can manage the application by deleting donors, hospitals, and organizations.


## Feedback and Contributions

Feel free to provide feedback and contributions to enhance the Blood Bank Application. Raise issues or submit pull requests in the GitHub repository.

---

Efficiently manage blood donation and distribution with the Blood Bank Application. Clone the repository or download the ZIP file, configure environment variables, install dependencies, and start the application. Explore tailored functionalities, analytics, and admin control in this MERN stack solution.
