# Delivery Dispatch Agent: Frontend (React + Vite)

    npm install
    npm run dev

Start the backend in a separate terminal first:

    cd ../backend
    npm run dev

For local development, the frontend's Vite server proxies `/api` requests to the backend on port `3000`.
If the frontend and backend are deployed on different origins, set `VITE_API_URL` in
`frontend/.env.local` (for example `https://your-backend.example.com`) and rebuild the frontend.
Sign in with the app passcode configured on the backend (`APP_PASSCODE`).

All data comes from the Next.js backend through `src/api/client.js` and refreshes every 10 seconds.
The map uses Leaflet with OpenStreetMap tiles (no API key needed).
