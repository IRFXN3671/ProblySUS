# Problysus - Scam Detection Web App

Problysus is a full-stack web application designed to analyze website URLs for potential scam risks. It provides a comprehensive risk assessment by performing multiple checks, including blacklist verification, domain age analysis, SSL certificate validation, and content trust verification.

## Key Features

- **Real-time URL Analysis**: Instantly scans URLs to detect potential threats.
- **Risk Scoring**: Calculates a risk score (0-100) and classifies sites as Safe, Suspicious, or Fraudulent.
- **Detailed Checks**:
  - **Blacklist Check**: Verifies if the domain is present in known threat intelligence feeds.
  - **WHOIS Analysis**: Checks domain age and creation date.
  - **SSL/HTTPS Verification**: Ensures the site uses a valid security certificate.
  - **Pattern Recognition**: Detects suspicious URL patterns often used in phishing.
  - **Content Trust**: Scans for essential trust indicators like Privacy Policy and Contact pages.

## Tech Stack

**Backend**
- Python
- Flask (Web Framework)
- `requests`, `python-whois` (Analysis Tools)

**Frontend**
- React (via Vite)
- Framer Motion (Animations)
- Axios (API Communication)

## Installation

### Prerequisites
- Python 3.8+
- Node.js & npm

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## How to Run

1. **Start the Backend Server**:
   From the `backend` directory (with venv activated):
   ```bash
   python app.py
   ```
   The backend will start on `http://127.0.0.1:5000`.

2. **Start the Frontend Development Server**:
   From the `frontend` directory:
   ```bash
   npm run dev
   ```
   Open the URL shown in the terminal (usually `http://localhost:5173`) to use the application.
