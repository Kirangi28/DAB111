Project Documentation

Folder Structure:

- instance/                # Configuration files (e.g., secret keys, database configurations)
- templates/               # HTML templates
  - index.html             # Main page template
- books_database/          # Main application package
  - run_app.py             # Flask application file
  - python_scrap/          # Script to extract data and populate the database
- books_database.db        # SQLite database file

How to Use:

1. Extracting Data and Populating the Database
The python_scrap folder contains a script designed to extract data from a website and populate the database named "books_database." To execute the script:

$ cd books_database/python_scrap
$ python scrape.py

This script updates the database with the latest information from the website.

2. Running the Flask Application
Open Command Prompt (cmd).
Navigate to the folder containing run_app.py.
Execute the following command to start the server:

$ python run_app.py

The Flask application will run locally, and you can access it by visiting http://127.0.0.1:5000/ in your web browser.

HTML Page (index.html):
The index.html file in the templates folder is the main page of the application. It displays a list of books retrieved from the database and includes a search bar for filtering books by name or price.


Flask Application (run_app.py):

The run_app.py file in the books_database folder serves as the Flask application. It connects to the SQLite database, retrieves data, and renders the index.html template.


Important Notes:
The database file (books_database.db) is automatically created and updated by the python_scrap script.
Ensure that all required libraries are installed by running pip install -r requirements.txt in your project directory.
Customize the HTML and Flask code according to your project requirements.

Additional Information:
For more details about Flask and its features, refer to the Flask Documentation.
This documentation provides a basic guide on how to use and understand the project structure. Customize it according to your specific needs and additional functionalities.

