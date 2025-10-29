# MERN Image Search & Multi-Select

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) application for searching and selecting multiple images from the Unsplash API.

## Features

- 🔍 **Image Search**: Search for images using the Unsplash API
- ✅ **Multi-Select**: Select multiple images with checkboxes
- 📱 **Responsive Design**: Works seamlessly on desktop and mobile devices
- 🎨 **Modern UI**: Clean and intuitive user interface
- 💾 **Persistent Storage**: Selected images are stored in MongoDB
- 🔄 **Real-time Updates**: Live feedback on selections

## Tech Stack

### Frontend
- React.js
- Axios for API calls
- CSS3 for styling

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- Unsplash API integration

## Project Structure

```
mern-image-search-multiselect/
├── client/                 # React frontend
│   ├── public/
│   └── src/
│       ├── components/
│       ├── App.js
│       └── index.js
├── server/                 # Express backend
│   ├── models/
│   ├── routes/
│   ├── config/
│   └── server.js
├── package.json
└── README.md
```

## Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- Unsplash API key

### Steps

1. Clone the repository:
```bash
git clone https://github.com/harshveer29/mern-image-search-multiselect.git
cd mern-image-search-multiselect
```

2. Install dependencies for both client and server:
```bash
# Install server dependencies
npm install

# Install client dependencies
cd client
npm install
cd ..
```

3. Create a `.env` file in the root directory:
```env
MONGO_URI=your_mongodb_connection_string
UNSPLASH_ACCESS_KEY=your_unsplash_api_key
PORT=5000
```

4. Start the development servers:
```bash
# Start backend server (from root)
npm run server

# Start frontend (in new terminal)
cd client
npm start
```

5. Open your browser and navigate to `http://localhost:3000`

## API Endpoints

### GET /api/images/search
Search for images from Unsplash
- Query params: `query` (search term)

### POST /api/selections
Save selected images to MongoDB
- Body: Array of image objects

### GET /api/selections
Get all saved selections

## Features Implementation

### 1. Image Search
- Users can enter search terms in the search bar
- Results are fetched from the Unsplash API
- Images are displayed in a responsive grid layout

### 2. Multi-Select Functionality
- Each image has a checkbox overlay
- Users can select/deselect multiple images
- Selected images are highlighted

### 3. Data Persistence
- Selected images are saved to MongoDB
- Users can view their saved selections
- Selections persist across sessions

## Environment Variables

| Variable | Description |
|----------|-------------|
| `MONGO_URI` | MongoDB connection string |
| `UNSPLASH_ACCESS_KEY` | Unsplash API access key |
| `PORT` | Server port (default: 5000) |

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Author

Harsh Veer Singh

## Acknowledgments

- Unsplash API for providing high-quality images
- MERN stack community for excellent documentation
- UD Studios for the assignment opportunity
