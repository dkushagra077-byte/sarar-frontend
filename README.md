# SARAR INDUSTRIES Frontend

React website frontend for SARAR INDUSTRIES, built with Webpack.

## Local development

1. Install dependencies: `npm ci`
2. Start the development server: `npm start`
3. The local dev server proxies `/api` requests to `http://localhost:5000`.

## Production build

Run `npm ci` followed by `npm run build`. The output is written to `dist/`. Production API requests default to `https://sarar-backend.onrender.com/api`. To use another API, set `REACT_APP_API_URL` before building; it must end in `/api`.

For a Render Static Site, use build command `npm ci && npm run build` and publish directory `dist`.

Configure the backend's `FRONTEND_URL` and `CORS_ORIGINS` with the deployed website's origin so browsers can call the API.

Production site URL: https://sarar-frontend.vercel.app/
The production build connects to https://sarar-backend.onrender.com/api.

## Vercel deployment

The included ercel.json sets the build output to dist and routes client-side paths to index.html for React Router.
