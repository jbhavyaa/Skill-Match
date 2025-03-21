# SkillMatch

SkillMatch is a MERN stack-based job portal designed to connect job seekers with recruiters. It provides authentication, job postings, and profile management functionalities with a responsive UI.

## Features
- **User Authentication**: Signup/Login for job seekers and recruiters.
- **Job Postings**: Recruiters can post, edit, and manage job listings.
- **Profile Management**: Users can update their resumes, skills, and job preferences.
- **Filtering and Searching**: Jobs can be filtered based on skills, experience, and location.
- **Secure Backend**: Uses authentication middleware for protected routes.
- **File Handling**: Supports resume uploads using Multer and Data URI encoding.

## Tech Stack
- **Frontend**: React (with Vite), TailwindCSS, ShadCN components
- **Backend**: Node.js, Express.js, MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **File Handling**: Multer, Data URI encoding

## Installation and Setup

### Prerequisites
Ensure you have the following installed:
- Node.js (>=16.x)
- MongoDB (local or cloud instance)
- Git

### Clone the Repository
```sh
git clone https://github.com/your-username/skillmatch.git
cd skillmatch
```

### Backend Setup
```sh
cd backend
npm install
```
Create a `.env` file in the backend directory and add:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```
Start the backend server:
```sh
npm start
```

### Frontend Setup
```sh
cd ../frontend
npm install
```
Create a `.env` file in the frontend directory and add:
```
VITE_API_URL=http://localhost:5000
```
Start the frontend server:
```sh
npm run dev
```

## Usage
1. Open `http://localhost:5173/` in your browser.
2. Register/Login as a job seeker or recruiter.
3. Recruiters can post jobs, while job seekers can browse and apply.
4. Manage profiles, update resumes, and track job applications.

## API Routes
### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login

### Jobs
- `POST /api/jobs` - Create a job (Recruiter only)
- `GET /api/jobs` - Get all jobs
- `GET /api/jobs/:id` - Get job by ID
- `PUT /api/jobs/:id` - Update job (Recruiter only)
- `DELETE /api/jobs/:id` - Delete job (Recruiter only)

## Contributing
Feel free to fork the repository and submit pull requests.

## License
This project is licensed under the MIT License.

## Contact
For any issues or feature requests, reach out via GitHub Issues or contact us at `bhavyajamar2004@gmail.com`.

