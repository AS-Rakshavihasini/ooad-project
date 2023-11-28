# Geovoyage Travel Budget Prediction System

## Overview

The Geovoyage Travel Budget Prediction System is a Flask web application that predicts travel budgets based on user input and suggests destinations within the predicted budget range. The system includes a trained machine learning model to make budget predictions and a database to manage user registration and login.

## Prerequisites

Before running the application, ensure you have the following:

- Python 3.x installed
- Required Python packages installed. You can install them using the following command:
  ```bash
  pip install Flask Flask-SQLAlchemy Flask-Login Flask-Bcrypt scikit-learn pandas
## Installation

1. **Clone the Repository:**

    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Application:**

    ```bash
    python app.py
    ```

    The application will be accessible at [http://localhost:5000](http://localhost:5000) in your web browser.

4. **Access the Application:**

    Visit [http://localhost:5000](http://localhost:5000) to access the Geovoyage application.

## Training the Model (Optional)

If you want to retrain the model, follow these steps:

1. Execute the training script:

    ```bash
    python train_model.py
    ```

    This script preprocesses the travel data, trains a linear regression model, and saves the trained model to `trained_model.joblib`.

2. The script will display the Mean Squared Error on the test set and generate a scatter plot of actual vs predicted values.

## Feedback Submission

Users can submit feedback through the "Contact Us" page. The feedback is processed and can be stored in a database for further analysis.

## Database

The application uses SQLite as its database. The database file (`site.db`) is created automatically when the application is run for the first time.

## User Authentication

User registration and authentication are implemented using Flask-Login and Flask-Bcrypt. Passwords are hashed before being stored in the database.

## About and Profile Pages

The application includes "About Us" and "Profile" pages to provide information about Geovoyage and allow logged-in users to view their profiles.

## Contact

For any inquiries or issues, please contact us through the "Contact Us" page in the application.

## Get Budget Prediction Page

Users can visit the "Get Budget Prediction" page to input their details and receive a travel budget prediction. The page includes a form with fields such as age, duration, cost of living, and more.

## See Destination Page

The "See Destination" page allows users to input their budget and receive suggestions for travel destinations within their specified budget range. Users can enter their budget, and the system will provide recommendations based on the available data.

For more detailed instructions and content, please refer to the respective files in the project's source code.

