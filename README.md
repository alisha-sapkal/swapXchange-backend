# SwapXchange Backend

## Deployment on Render

- Ensure you set the following environment variables in Render:
  - `PORT` (Render sets this automatically)
  - `MONGODB_URI` (or your DB connection string)
  - `CLIENT_ORIGIN` (set this to your deployed frontend URL, e.g., https://swap-xchange-ui-c5jf.vercel.app/)
  - Any other secrets (JWT, etc.)

- The backend will listen on the port provided by Render.
- CORS is configured to allow requests from the domain set in `CLIENT_ORIGIN`.
