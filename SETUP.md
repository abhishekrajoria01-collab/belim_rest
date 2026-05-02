# Setup Instructions

## Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- npm or yarn

## Step 1: Clone and Navigate

```bash
git clone https://github.com/abhishekrajoria01-collab/belim_rest.git
cd belim_rest
```

## Step 2: Install All Dependencies

```bash
npm run install:all
```

This will install:
- Root dependencies
- Server dependencies
- Client dependencies

## Step 3: Configure Environment Variables

### Server Configuration

Create `server/.env`:

```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/attendance_tracker
JWT_SECRET=your_jwt_secret_key_here
NODE_ENV=development
CLIENT_URL=http://localhost:3000
```

### Client Configuration

Create `client/.env.local`:

```
REACT_APP_API_URL=http://localhost:5000
REACT_APP_API_TIMEOUT=10000
```

## Step 4: Start MongoDB

```bash
# If MongoDB is installed locally
mongod

# Or use MongoDB Atlas (update MONGODB_URI in .env)
```

## Step 5: Run the Application

```bash
# Development mode
npm run dev

# This will start both server and client concurrently
```

## Step 6: Access the Application

- **Frontend:** http://localhost:3000
- **Backend API:** http://localhost:5000
- **API Documentation:** http://localhost:5000/api-docs

## Troubleshooting

### MongoDB Connection Error
- Ensure MongoDB is running
- Verify MONGODB_URI in server/.env
- Check network connectivity if using Atlas

### Port Already in Use
- Change PORT in server/.env
- Or kill process using the port

### Module Not Found
- Run `npm run install:all` again
- Delete node_modules and reinstall

## Next Steps

1. Create admin user
2. Add employees to the system
3. Start marking attendance
4. Generate reports

For more details, see the main [README.md](./README.md)
