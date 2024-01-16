# Web authentication

This repository contains a simple web authentication workflow using [Auth0](https://developer.auth0.com/).

## Getting started

### Installation

1. Install backend dependencies

```shell
cd backend
npm install
```

2. Create `.env` file in `backend/` with the following variables:

```shell
PORT=6060
CLIENT_ORIGIN_URL=http://localhost:4040
AUTH0_AUDIENCE=<your Auth0 app audience>
AUTH0_DOMAIN=<your Auth0 app domain>
```

3. Install frontend dependencies

```shell
cd frontend
npm install
```

4. Create `.env` file in `frontend/` with the following variables:

```shell
REACT_APP_AUTH0_DOMAIN=<your Auth0 app domain>
REACT_APP_AUTH0_CLIENT_ID=<your Auth0 app client id>
REACT_APP_AUTH0_CALLBACK_URL=http://localhost:4040/callback
REACT_APP_AUTH0_AUDIENCE=<your Auth0 app audience>
REACT_APP_API_SERVER_URL=http://localhost:6060
```

### Running the app locally

To run the authentication app locally:

1. Start the backend server

```shell
cd backend
npm run dev
```

2. Start the frontend client

```shell
cd frontend
npm start
```

3. Navigate to `http://localhost:4040/`
