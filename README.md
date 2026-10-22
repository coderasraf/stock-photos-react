# Stock Photos

A React photo gallery that loads images from the Unsplash API and keeps loading more as you scroll.

![React](https://img.shields.io/badge/React-16-61DAFB?logo=react&logoColor=white)
![Unsplash](https://img.shields.io/badge/Unsplash-API-000000?logo=unsplash&logoColor=white)

## About

Built in 2022 as a learning project while practicing React hooks (`useState`, `useEffect`), async data fetching and scroll events, based on the "Stock Photos" exercise from John Smilga's React projects course.

## Features

- Fetches the latest photos from the Unsplash `/photos` endpoint
- Infinite scroll: requests the next page when you reach the bottom of the page
- Photo cards with the image, photographer name, like count and avatar linking to their portfolio
- Loading indicator while new photos are fetched
- Search bar UI (search is not wired up yet)

## Tech Stack

- React 16 (Create React App)
- Fetch API + Unsplash REST API
- React Icons

## Getting Started

Prerequisites: Node.js, npm and a free [Unsplash developer](https://unsplash.com/developers) access key.

```bash
git clone https://github.com/coderasraf/stock-photos-react.git
cd stock-photos-react
npm install
```

Create a `.env` file in the project root:

```bash
REACT_APP_ACCESS_KEY=your_unsplash_access_key
```

Then run:

```bash
npm start        # http://localhost:3000
npm run build    # production build
```

## Environment Variables

| Name | Purpose |
| --- | --- |
| `REACT_APP_ACCESS_KEY` | Unsplash API access key (sent as `client_id`) |

## Project Structure

```text
src/
├── App.js     # Fetching, infinite scroll, search form
├── Photo.js   # Single photo card
├── index.css
└── index.js
```

## Author

Built by **Ashraf Siddik**, Shopify developer & CRO specialist.
- Website: [ashraf-siddik.com](https://ashraf-siddik.com)
- GitHub: [@coderasraf](https://github.com/coderasraf)
