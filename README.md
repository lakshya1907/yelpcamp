# YelpCamp 🏕️

A full-stack campground review platform built with Node.js, Express, MongoDB, and Mapbox. Discover, share, and review campgrounds across the country.

## Features

- 🗺 **Interactive cluster map** — browse all campgrounds on a live Mapbox map
- 📸 **Photo galleries** — upload multiple images per campground via Cloudinary
- ⭐ **Star ratings & reviews** — leave and manage reviews
- 🔐 **Authentication** — secure register/login with Passport.js
- 🛡 **Authorization** — only owners can edit/delete their campgrounds
- 📱 **Responsive design** — works beautifully on all screen sizes

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js + Express |
| Database | MongoDB + Mongoose |
| Views | EJS + ejs-mate |
| Auth | Passport.js (local strategy) |
| Maps | Mapbox GL JS |
| Images | Cloudinary + Multer |
| Validation | Joi |

## Getting Started

### Prerequisites

- Node.js v14+
- MongoDB (local or Atlas)
- Cloudinary account
- Mapbox account

### Installation

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/YelpCamp.git
cd YelpCamp

# Install dependencies
npm install

# Create a .env file
touch .env
```

### Environment Variables

Create a `.env` file in the root directory:

```
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_KEY=your_api_key
CLOUDINARY_SECRET=your_api_secret
MAPBOX_TOKEN=your_mapbox_token
DB_URL=mongodb://localhost:27017/yelp-camp
SECRET=your_session_secret
```

### Run the App

```bash
# Seed the database (optional)
node seeds/index.js

# Start the server
npm start
```

Visit `http://localhost:3000`

## Project Structure

```
YelpCamp/
├── app.js              # Entry point
├── controllers/        # Route logic
├── models/             # Mongoose models
├── routes/             # Express routers
├── views/              # EJS templates
│   ├── campgrounds/    # Campground pages
│   ├── users/          # Auth pages
│   ├── layouts/        # Base layout
│   └── partials/       # Reusable components
├── public/             # Static assets
│   ├── stylesheets/    # CSS
│   └── javascripts/    # Client-side JS
├── seeds/              # Database seed data
└── utils/              # Helpers
```

## License

MIT
