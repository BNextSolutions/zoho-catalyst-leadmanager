# Zoho Catalyst Lead Manager

A web application built with Zoho Catalyst for managing leads in Zoho CRM.

## Project Structure

```
zoho-catalyst-leadmanager/
├── functions/
│   └── crm_crud/         # Backend API functions
├── leadmanager-app/      # Frontend React application
└── README.md
```

## Prerequisites

- Zoho Catalyst account
- Zoho CRM account
- Node.js and npm installed
- Zoho Catalyst CLI

## Setup

1. Install Zoho Catalyst CLI globally:
```bash
npm install -g zcatalyst-cli
```

2. Install project dependencies:
```bash
# Install backend dependencies
cd functions/crm_crud
npm install

# Install frontend dependencies
cd ../../leadmanager-app
npm install
```

3. Configure your environment variables:
   - Create `.env` file in `functions/crm_crud`
   - Add your Zoho CRM credentials:
```env
ZOHO_CLIENT_ID=your_client_id
ZOHO_CLIENT_SECRET=your_client_secret
ZOHO_REFRESH_TOKEN=your_refresh_token
```

## Development

To run the application locally:

1. Start the backend:
```bash
cd functions/crm_crud
catalyst serve
```

2. Start the frontend:
```bash
cd leadmanager-app
npm start
```

## Features

- Connect to Zoho CRM using OAuth2.0
- View all leads
- Create new leads
- Update existing leads
- Delete leads

## Deployment

To deploy to Zoho Catalyst:

```bash
# Deploy backend functions
cd functions/crm_crud
catalyst deploy

# Build and deploy frontend
cd ../../leadmanager-app
npm run build
catalyst deploy
```

## Tech Stack

- Backend: Node.js with Zoho Catalyst Functions
- Frontend: React.js
- API: Zoho CRM REST API
- Authentication: OAuth 2.0

## License

This project is licensed under the MIT License. 