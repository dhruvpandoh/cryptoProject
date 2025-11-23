# CryptoProject (CryptoShow Dashboard)

A full-stack crypto dashboard similar to `crypto-main`, featuring live prices via Coinlayer and a MongoDB-backed save/list system.

## Features
- Live crypto list + market rates from Coinlayer
- Paginated browsing + search
- Save crypto items to MongoDB backend
- CRUD operations exposed through Express routes

## Tech Stack
- React (CRA)
- Material UI / MUI
- Node.js + Express
- MongoDB + Mongoose
- Axios, Lodash

## Folder Structure
```
cryptoProject-main/
  Backend/        # Express APIs
  cryptoshow/     # React frontend
```

## Running Locally

### Backend
```bash
cd cryptoProject-main/Backend
npm install
npm run dev
```
Runs at `http://localhost:5000`

### Frontend
```bash
cd ../cryptoshow
npm install
npm start
```
Runs at `http://localhost:3000`

## API Routes
- `GET /api/crypto/fetchalldata`
- `POST /api/crypto/savecrypto`
- `PUT /api/crypto/updatecrypto/:id`
- `DELETE /api/crypto/deletecrypto/:id`

## Notes
- The Coinlayer API key is embedded in `Home.js`.  
  Move to `.env` for production safety.

## Future Improvements
- Add visualizations (sparkline charts).
- Portfolio summaries (total value, P/L).
