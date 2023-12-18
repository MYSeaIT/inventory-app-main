# inventory-app

A full-stack application to track your inventory.

## Description

This project is a full-stack web application that allows users to manage an inventory of products, particularly sauces. The backend is built with Express.js server and communicates with the frontend created in React.

## Getting Started

1. Install all the required packages using `npm install`.
2. Populate the database with initial data using `npm run seed`.
3. Start the Express server with `npm run server-dev`.
4. Open another terminal and start the React development server with `npm run client-dev`.

## Troubleshooting

### Common Errors

Below are some of the common errors you might encounter while working on the `inventory-app` along with troubleshooting steps:

#### Database Syncing Issues

- Error: Sequelize connection error.
- Cause: The database is not running or `.env` file is not set up correctly with the correct database credentials.
- Solution: Ensure that the database service is running and that the `.env` file contains the correct database URL.

#### Module Not Found

- Error: `Error: Cannot find module 'xyz'` where `xyz` is a module.
- Cause: Dependency not installed or an incorrect import statement.
- Solution: Run `npm install` to ensure all dependencies are installed. Check the import statement for typos.

#### CORS Issues

- Error: Cross-Origin Resource Sharing (CORS) errors in the browser's console.
- Cause: The frontend makes requests to a domain different from the one served by the backend.
- Solution: Ensure `cors` middleware is included and configured correctly in `server/app.js`.

### Specific Errors

#### API Route Not Found

If an API call to a non-existing route is made, you will encounter an error:

- Error: `404 - Not Found`
- Cause: The client made a request to an endpoint that does not exist.
- Solution: Check the fetch URL in the React component and verify that it matches a defined route in `server/routes/index.js`.

#### Fetch Call Errors in React Component

- Error: Network request failed or similar errors in the console when making a fetch call from the React component.
- Cause: API server is not running or the endpoint is incorrect.
- Solution: Ensure the API server is running (`npm run server-dev`). Check the endpoint in the `fetchSauces` function within the `App.js` component.

## Contributing

For contributing to this project, please follow the next steps:

1. Fork the repository.
2. Create a new branch for your feature.
3. Commit changes to the branch.
4. Push the branch to GitHub.
5. Submit a pull request to the main branch.



