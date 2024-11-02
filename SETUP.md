# Setup Instructions

Follow these steps to get the repository up and running:

## Prerequisites

- Docker
- Docker Compose
- Node.js
- npm or yarn
- Python 3.x
- pip

## Clone the Repository

```bash
git clone https://github.com/yourusername/software-engineering-group24-25-14.git
cd software-engineering-group24-25-14
```

## Backend Setup (Django)

1. Create a virtual environment and activate it:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

2. Install the required Python packages:

   ```bash
   pip install -r backend/requirements.txt
   ```

3. Run database migrations:

   ```bash
   python backend/manage.py migrate
   ```

## Frontend Setup (Next.js)

1. Navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install the required Node.js packages:

   ```bash
   npm install
   # or
   yarn install
   ```

## Database Setup (PostgreSQL with Docker)

1. Navigate back to the root directory:

   ```bash
   cd ..
   ```

2. Start the PostgreSQL container:

   ```bash
   docker-compose up -d
   ```

## Running the Application

1. Start the Django development server:

   ```bash
   python backend/manage.py runserver
   ```

2. Start the Next.js development server:

   ```bash
   cd frontend
   npm run dev
   # or
   yarn dev
   ```

Your application should now be running with the Django backend and Next.js frontend.
