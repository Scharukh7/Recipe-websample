# Recipe-websample

## Overview

This project is a web-based recipe management application built with React.js for the frontend and Django for the backend. The application allows users to browse and manage a collection of recipes, and is designed to showcase a vibrant, user-friendly interface.

## Features

- **Dynamic Recipe Cards**: Displayed in a responsive card layout.
- **Task Management**: Full CRUD functionality for tasks (represented as recipes).
- **Real-time Interaction**: Seamless communication between the frontend and backend.
- **3-Tier Architecture**: Designed for scalability and high availability using AWS services.

## Project Structure

- **Frontend**: React.js
- **Backend**: Django and Django REST Framework
- **Database**: SQLite (for development purposes)

## Prerequisites

Ensure you have the following installed on your system:

- Python 3.x
- Node.js and npm
- pip (Python package installer)

## Setup Instructions

### 1. Backend Setup (Django)

1. **Clone the repository**:

    ```bash
    git clone <your-repo-link>
    cd <your-repo-directory>/todobackend
    ```

2. **Create and activate a virtual environment**:

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    ```

3. **Install the required Python packages**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply the migrations to set up the database**:

    ```bash
    python manage.py migrate
    ```

5. **Run the Django development server**:

    ```bash
    python manage.py runserver
    ```

### 2. Frontend Setup (React.js)

1. **Navigate to the frontend directory**:

    ```bash
    cd <your-repo-directory>/todo-list
    ```

2. **Install the required npm packages**:

    ```bash
    npm install
    ```

3. **Start the React development server**:

    ```bash
    npm start
    ```

### 3. Accessing the Application

- **Frontend**: Open [http://localhost:3000](http://localhost:3000) in your web browser.
- **Backend API**: The API can be accessed at [http://localhost:8000/api/tasks/](http://localhost:8000/api/tasks/).

## AWS 3-Tier Architecture

The application is designed to be deployed using AWS services:

1. **Presentation Layer**: React.js frontend hosted on Amazon S3 with CloudFront for content delivery.
2. **Application Layer**: Django backend hosted on Amazon EC2 or AWS Elastic Beanstalk.
3. **Data Layer**: Task data managed using Amazon RDS.

## Contributing

Feel free to fork this repository and submit pull requests if you have any improvements or bug fixes.

## License

This project is licensed under the MIT License.
