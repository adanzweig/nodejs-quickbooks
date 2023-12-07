# QuickBooks Integration Example

This Node.js application demonstrates a basic integration with the QuickBooks Online API using OAuth for authentication. It shows how to authenticate with QuickBooks, retrieve an access token, and make API calls to fetch payment data.

## Prerequisites

Before you begin, ensure you have the following:

- Node.js installed on your machine.
- A QuickBooks Online account.
- A QuickBooks Online app with Client ID and Client Secret.

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/adanzweig/nodejs-quickbooks
cd nodejs-quickbooks
npm install
```

## Configuration

Create a `.env` file in the root directory of the project and add the following variables:

```env
CLIENT_ID=your_quickbooks_client_id
CLIENT_SECRET=your_quickbooks_client_secret
ENVIRONMENT=sandbox # or 'production'
REDIRECT_URL=your_oauth_redirect_uri
```

## Running the Application

Start the server:

```bash
npm start
```

The server will start on `http://localhost:3000`.

## Usage

1. Navigate to `http://localhost:3000/auth` to initiate the OAuth flow.
2. Log in to your QuickBooks account and authorize the application.
3. You will be redirected to the `/payments` route, where the application will display payment data from QuickBooks.

## Features

- OAuth integration with QuickBooks Online.
- Fetch and display payment data from QuickBooks Online.

## Contributing

Feel free to fork the repository and submit pull requests.

## Acknowledgments

- QuickBooks Online API
- Node.js community