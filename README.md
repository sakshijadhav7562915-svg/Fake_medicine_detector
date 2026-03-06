# Fake Medicine Detector

A web application that helps detect counterfeit medicines using image analysis and machine learning. This project provides a user-friendly interface for uploading medicine images and getting instant analysis results.

## Features

- 📸 Image upload and analysis
- 🔍 Real-time medicine verification
- 📊 Confidence scoring system
- 📱 Responsive design
- 🔒 Secure MongoDB storage
- 🚀 Fast and efficient processing

## Tech Stack

- **Frontend:**
  - HTML5
  - CSS3
  - JavaScript (ES6+)
  - Modern UI/UX design

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB
  - Multer (for file handling)

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- MongoDB (v4.4 or higher)
- npm (Node Package Manager)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Fake_medicine_detector.git
cd Fake_medicine_detector
```

2. Install dependencies:
```bash
npm install
```

3. Set up MongoDB:
   - Make sure MongoDB is running on your system
   - The application will connect to `mongodb://localhost:27017/medicine_detector`

4. Start the server:
```bash
node backend/app.js
```

5. Open the application:
   - Navigate to `http://localhost:3000` in your web browser

## Project Structure

```
Fake_medicine_detector/
├── src/                    # Frontend source code
│   ├── components/         # React components
│   ├── pages/             # Page components
│   ├── context/           # React context
│   ├── utils/             # Utility functions
│   ├── styles.css         # Global styles
│   ├── App.tsx           # Main App component
│   └── main.tsx          # Entry point
├── backend/               # Backend server (Express.js)
│   ├── routes/           # API routes
│   ├── middleware/       # Express middleware
│   ├── models/           # Database models
│   ├── services/         # Business logic
│   └── config/           # Configuration files
├── ml_model/             # Machine Learning models
│   ├── MODELS/           # Trained models
│   └── real_medicines/   # Training data
├── .venv/                # Python virtual environment
├── node_modules/         # Node.js dependencies
├── public/              # Static files
└── package.json         # Node.js project configuration
```

## Setup Instructions

1. **Frontend Setup**
   ```bash
   npm install
   npm run dev
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   npm start
   ```

3. **ML Model Setup**
   ```bash
   cd ml_model
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   pip install -r requirements.txt
   ```

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```
MONGODB_URI=your_mongodb_uri
PORT=3000
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## API Endpoints

- `GET /api/test` - Test backend connection
- `POST /api/upload` - Upload medicine image
- `GET /api/medicines` - Get all uploaded medicines
- `GET /api/medicines/:id` - Get specific medicine image

## Usage

1. Open the application in your web browser
2. Click "Choose Medicine Image" to select an image
3. Click "Upload and Analyze" to process the image
4. View the analysis results and confidence score
5. Browse previously uploaded images in the gallery

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Security

- All uploaded images are stored securely in MongoDB
- File type validation ensures only image files are processed
- CORS is enabled for secure cross-origin requests

## Future Enhancements

- [ ] Implement machine learning model for better detection
- [ ] Add user authentication
- [ ] Support for batch image processing
- [ ] Detailed analysis reports
- [ ] Mobile application version

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to all contributors who have helped shape this project
- Special thanks to the open-source community for their invaluable tools and libraries

## Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter)
Project Link: [https://github.com/yourusername/Fake_medicine_detector](https://github.com/yourusername/Fake_medicine_detector) vv