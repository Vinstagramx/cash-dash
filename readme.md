# CashDash - Personal Finance Dashboard

CashDash is a web-based application designed to help users track their personal finances, set budgeting and other financial goals, and integrate with external services such as Splitwise, bank accounts, and investment apps. This application utilizes Golang for the backend, MongoDB as the database, and React.js for the frontend.

## Features

- **Financial Tracking**: The dashboard allows users to input and track their income, expenses, and overall financial transactions. Users can categorize transactions, view summaries, and analyze their spending patterns.

- **Budgeting Goals**: Users can set budgeting goals based on different categories (e.g., groceries, entertainment) and track their progress. The dashboard provides visualizations and alerts to help users stay on track with their financial goals.

- **Integration with Splitwise**: Integration with Splitwise enables users to sync shared bills and expenses, making it easier to manage shared finances and track individual contributions.

- **External Account Integration**: The dashboard supports integration with external bank accounts and investment apps, allowing users to view their account balances, portfolio performance, and transaction history within the application. This will then update the database periodically, based on the availability or pricing plans of external APIs.

## Architecture

The Personal Finance Dashboard follows a client-server architecture:

- **Backend**: The backend of the application is developed using Golang. It provides RESTful APIs to handle user authentication, financial data management, goal tracking, and integration with external services. The backend interacts with a local MongoDB database to store user data securely.

- **Frontend**: The frontend is built using React.js, a popular JavaScript library for building user interfaces. It consumes the backend APIs to fetch and display data, enabling users to interact with their financial information, set goals, and visualize their finances using charts and graphs.

## Getting Started

To run the Personal Finance Dashboard locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/personal-finance-dashboard.git
   ```

2. Set up the backend:
   - Install Golang and MongoDB on your system if not already done.
   - Navigate to the backend directory:
     ```bash
     cd personal-finance-dashboard/backend
     ```
   - Install dependencies:
     ```bash
     go mod download
     ```
   - Set up environment variables by creating a `.env` file:
     ```
     MONGO_URI=your_mongodb_uri
     SECRET_KEY=your_secret_key
     ```
   - Start the backend server:
     ```bash
     go run main.go
     ```

3. Set up the frontend:
   - Ensure you have Node.js and npm (Node Package Manager) installed.
   - Navigate to the frontend directory:
     ```bash
     cd personal-finance-dashboard/frontend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the frontend development server:
     ```bash
     npm start
     ```

4. Open the application in your browser:
   - Access the application by visiting `http://localhost:3000` in your preferred browser.

## Contribution

Contributions to the Personal Finance Dashboard project are welcome! If you would like to contribute, please follow these steps:

1. Fork the repository on GitHub.
2. Create a new branch with a descriptive name:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes with clear and concise commit messages:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push your branch to your forked repository:
   ```bash
   git push origin feature/new-feature
   ```
5. Open a pull request on the main repository, describing your changes in detail.

## License

This project is licensed under the [MIT

 License](LICENSE).

---

This README.md file will be expanded or refined as the project develops.