# File Sharing Application

A modern MERN stack application for secure file upload and sharing. Users can upload files and get shareable download links with download tracking.

## Features

- 📁 **File Upload**: Upload files up to 10MB
- 🔗 **Share Links**: Get instant shareable download links
- 📊 **Download Tracking**: Track how many times files are downloaded
- 🎨 **Modern UI**: Clean and responsive user interface
- 🔒 **Secure**: File validation and error handling

## Tech Stack

**Frontend:**
- React 18
- Axios for API calls
- CSS3 for styling

**Backend:**
- Node.js with Express
- MongoDB with Mongoose
- Multer for file uploads
- CORS enabled

## Usage

1. **Upload a File**: Click the "Upload" button and select a file (max 10MB)
2. **Get Share Link**: After upload, you'll receive a shareable download link
3. **Share & Download**: Share the link with others for file downloads
4. **Track Downloads**: Each download is automatically tracked in the database
![Alt text](projectimage1.png)
![Alt text](projectimage2.png)


## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/upload` | Upload a file |
| GET | `/file/:fileId` | Download a file by ID |

## Project Structure

```
AlgoU-MERN-File-Sharing-Application/
├── client/                 # React frontend
│   ├── src/
│   │   ├── service/       # API service functions
│   │   ├── App.js         # Main React component
│   │   └── App.css        # Styling
│   └── package.json
├── server/                # Node.js backend
│   ├── controller/        # Route controllers
│   ├── database/         # Database connection
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API routes
│   ├── utils/            # Utility functions
│   ├── uploads/          # File storage directory
│   ├── .env.example      # Environment variables template
│   └── package.json
└── README.md
```

## Dependencies

### Backend Dependencies
- express: Web framework for Node.js
- mongoose: MongoDB object modeling
- multer: File upload middleware
- cors: Cross-origin resource sharing
- dotenv: Environment variable management

### Frontend Dependencies
- react: UI library
- axios: HTTP client for API calls
