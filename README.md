# Novatech Website

## Overview
This repository contains the codebase for the Novatech corporate website. Novatech specializes in cutting-edge technology solutions and services for enterprise clients.

## Features
- Responsive design optimized for desktop, tablet, and mobile devices
- Product showcase with detailed specifications
- Interactive service catalog
- Client testimonials and case studies
- Contact forms with validation
- News and blog section
- Career opportunities page

## Technologies
- Frontend: HTML5, CSS3, JavaScript, React.js
- State Management: Redux
- Styling: Sass/SCSS, Tailwind CSS
- Backend: Node.js, Express
- Database: MongoDB
- Authentication: JWT
- Deployment: Docker, AWS

## Prerequisites
- Node.js (v16.x or later)
- npm (v8.x or later)
- MongoDB (v5.x or later)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/novatech/website.git
cd website
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with the following variables:
```
PORT=3000
MONGODB_URI=mongodb://localhost:27017/novatech
JWT_SECRET=your_jwt_secret
NODE_ENV=development
```

4. Start the development server:
```bash
npm run dev
```

## Project Structure
```
novatech-website/
├── client/                 # Frontend React application
│   ├── public/             # Static files
│   ├── src/                # Source files
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── assets/         # Images, fonts, etc.
│   │   ├── styles/         # Global styles
│   │   ├── utils/          # Utility functions
│   │   └── App.js          # Main application component
├── server/                 # Backend Node.js/Express application
│   ├── controllers/        # Request handlers
│   ├── models/             # Database models
│   ├── routes/             # API endpoints
│   ├── middleware/         # Custom middleware
│   └── server.js           # Entry point
├── .env                    # Environment variables
├── .gitignore              # Git ignore file
├── package.json            # Project dependencies
└── README.md               # This file
```

## Available Scripts
- `npm run dev`: Starts both frontend and backend in development mode
- `npm run client`: Starts only the frontend in development mode
- `npm run server`: Starts only the backend in development mode
- `npm run build`: Builds the frontend for production
- `npm start`: Starts the production server
- `npm test`: Runs tests
- `npm run lint`: Lints the codebase

## Deployment
The application is containerized using Docker and can be deployed on any cloud platform that supports Docker containers.

### Docker Deployment
```bash
# Build the Docker image
docker build -t novatech-website .

# Run the container
docker run -p 3000:3000 novatech-website
```

### AWS Deployment
Refer to the deployment documentation in `docs/deployment-aws.md` for detailed instructions on deploying to AWS.

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For any questions or support, please email developers@novatech.com or open an issue on GitHub.
