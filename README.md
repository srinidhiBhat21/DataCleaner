# Data Cleaning Application

A modern web application for cleaning and standardizing CSV data files. This tool provides an intuitive interface for uploading CSV files and automatically handles common data issues such as missing values, duplicates, inconsistent formatting, and more.

## Features

- Automatic detection and handling of missing values
- Duplicate record identification and removal
- Whitespace trimming
- Case standardization
- Data type detection and conversion
- Outlier detection
- Interactive data preview
- Downloadable clean data and processing logs

## Project Structure

```
dataclean/
├── backend/               # Flask API server
│   ├── app.py             # Main server file
│   ├── data_cleaning_bot.py  # Data cleaning logic
│   ├── requirements.txt   # Python dependencies
│   ├── uploads/           # Temporary storage for uploaded files
│   └── cleaned/           # Output directory for cleaned files
├── frontend/              # Web interface
│   ├── index.html         # Main HTML file
│   ├── css/
│   │   └── style.css      # Styling
│   └── js/
│       └── app.js         # Frontend logic
└── README.md              # This file
```

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- Node.js and npm (optional, for development)

### Backend Setup

1. Navigate to the backend directory:
   ```
   cd backend
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows:
     ```
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

5. Start the Flask server:
   ```
   python app.py
   ```
   The backend server will run on http://localhost:5000

### Frontend Setup

1. Navigate to the frontend directory:
   ```
   cd frontend
   ```

2. Start a simple HTTP server:
   - Using Python:
     ```
     python -m http.server 8080
     ```
   - Using Node.js (if installed):
     ```
     npx serve -l 8080
     ```

3. Open your browser and go to:
   ```
   http://localhost:8080
   ```

## How to Use

1. Open your browser and navigate to http://localhost:8080
2. Drag and drop a CSV file or click to select a file
3. Choose the cleaning options or use the default settings
4. Click "Clean My Data"
5. Review the results in the interactive dashboard
6. Download the cleaned CSV file and/or processing log

## Test Files

The repository includes some sample CSV files for testing:

- `simple_test.csv` - A clean CSV file for reference
- `simple_dirty_test.csv` - A CSV with common data issues to test cleaning features
- `test_data_comprehensive.csv` - A more complex file with various data problems

## Troubleshooting

- Make sure both the backend (port 5000) and frontend (port 8080) servers are running
- Check browser console for any JavaScript errors
- Verify that the CSV file format is valid
- Ensure your Python environment has all required dependencies installed

## License

MIT

## Contributors

