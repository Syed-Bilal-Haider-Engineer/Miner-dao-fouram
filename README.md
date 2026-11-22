# Miner Dao Forum

Discussion forum for Miner Dao. The React app covers posts, comments, polls, profiles, and admin review. The Express API stores data in MongoDB and can serve the production build.

## Project layout

- `src/` — React client
- `server/` — Express API, Mongoose models, and routes
- `public/` — static HTML and manifest
- `config-overrides.js` — Create React App webpack overrides

## Frontend

From the project root:

```bash
npm install
npm start
```

The app opens at [http://localhost:3000](http://localhost:3000).

Other scripts:

- `npm run build` — production build
- `npm test` — tests

## Backend

From `server/`:

```bash
npm install
npm run dev
```

The API listens on `PORT`, or port `4000` when `PORT` is not set. `npm start` runs the server without nodemon.

## Main areas

- Auth: signup, login, email verification, password reset
- Discussions: create, edit, like, search, categories
- Comments and replies, including mentions
- Polls and votes
- User profile: posts, likes, votes, mentions
- Admin: pending, approved, and rejected posts
- Wallet connect on BSC testnet
