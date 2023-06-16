# BuyCars Attryb Backend

The backend is implemented using Node.js with Express.js as the web framework. It utilizes MongoDB as the database for storing car listings and user information. And all of these are done in Typescript. The backend dependencies include:
## Dependencies
- **bcrypt**: Password hashing library.
- **cors**: Middleware for enabling CORS in Express apps.
- **dotenv**: Environment variable loader.
- **express**: Fast, unopinionated, minimalist web framework for Node.js.
- **jsonwebtoken**: JSON Web Token implementation.
- **mongoose**: MongoDB object modeling tool.
- **nodemon**: Utility for automatically restarting the server during development.

## API Routes

The following table lists the available API routes and their descriptions:

| Route             | Method | Description                                                    |
|-------------------|--------|----------------------------------------------------------------|
| user/signup/      | POST   | Register user data in the database                             |
| user/signin/      | POST   | Authenticate user credentials and allow them to log in         |
| marketplace/      | GET    | Retrieve all available cars for sale                           |
| marketplace/      | POST   | Post a new car for sale in the marketplace                     |
| marketplace/:carId | PATCH  | Update specific car details (only allowed for dealers)         |
| marketplace/:carId | DELETE | Delete specific car (only allowed for dealers)                 |
| oemspec/          | GET    | Retrieve the list of Original Equipment Manufacturers (OEMs)   |
| oemspec/          | POST   | Add new Original Equipment Manufacturer's data to the database |
