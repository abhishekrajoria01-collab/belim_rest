# Belim Attendance Tracker

A comprehensive web and mobile attendance tracking application for managing employee attendance with real-time status updates, date tracking, timestamps, and PDF reports.

## Features

✅ **Employee Attendance Management**
- Mark attendance status (Present, Absent, Shift)
- Real-time status updates
- Timestamp recording for each action

✅ **Date & Time Tracking**
- Daily attendance calendar
- Time-based punch in/out
- Shift management

✅ **Database Storage**
- Persistent employee data
- Complete attendance history
- Secure data management

✅ **Reports & Analytics**
- Attendance reports with statistics
- PDF export functionality
- Monthly/weekly summaries

✅ **Responsive UI**
- Web application
- Mobile-friendly design
- Intuitive user interface

## Tech Stack

### Backend
- Node.js + Express.js
- MongoDB
- JWT Authentication

### Frontend
- React.js
- TailwindCSS
- Axios for API calls
- React-PDF for report generation

## Project Structure

```
belim_rest/
├── server/              # Backend API
│   ├── models/          # Database models
│   ├── routes/          # API routes
│   ├── controllers/      # Business logic
│   ├── middleware/       # Authentication & validation
│   └── config/          # Configuration files
├── client/              # Frontend React app
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Page components
│   │   ├── services/    # API services
│   │   └── utils/       # Utility functions
│   └── public/          # Static files
└── README.md
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/abhishekrajoria01-collab/belim_rest.git
cd belim_rest
```

2. Install dependencies:
```bash
npm run install:all
```

3. Setup environment variables:
```bash
cp server/.env.example server/.env
cp client/.env.example client/.env
```

4. Run the application:
```bash
npm run dev
```

## Usage

- **Server runs on:** http://localhost:5000
- **Client runs on:** http://localhost:3000

## API Documentation

See [API Documentation](./server/API.md) for detailed endpoint information.

## Contributing

Feel free to submit issues and pull requests.

## License

ISC
