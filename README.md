# Weather API Builder

## Overview

The Weather API Builder is a Flask web application that allows users to access historical temperature data from various weather stations through a simple API. With this tool, users can retrieve temperature information from specific stations, dates, or years. The project is powered by data collected from weather stations stored in a series of text files.

## Features

- **Station Selection**: Users can choose a specific weather station based on its ID.

- **Date-Based Queries**: Retrieve temperature data for a specific date.

- **Yearly Data**: Get temperature data for an entire year from the selected station.

- **API Endpoints**: The application offers multiple API endpoints to access temperature data efficiently.

- **User-Friendly**: The user interface provides examples and URLs for easy API access.

## How to Use

1. Ensure you have Python installed on your system.

2. Install the required libraries using `pip install flask pandas`.

3. Download the weather station data files and store them in the `data_small` folder.

4. Run the Flask application by executing `python main.py` in the command line.

5. Access the API using the following endpoints:

   - `/api/v1/<station>/<date>`: Retrieve temperature data for a specific station and date.
   
     Example: http://127.0.0.1:5001/api/v1/10/1988-10-25

   - `/api/v1/<station>`: Get all temperature data for a specific station.
   
     Example: http://127.0.0.1:5001/api/v1/10

   - `/api/v1/yearly/<station>/<year>`: Fetch temperature data for an entire year from a station.
   
     Example: http://127.0.0.1:5001/api/v1/yearly/10/1988

## Prerequisites

- Python installed on your system.

- Required Python libraries: Flask and pandas. Install these libraries using pip if not already installed.

- Weather station data files stored in the `data_small` folder.

## License

This project is licensed under the MIT License. You are free to use and modify the code for your own purposes.

## Notes

- The project provides a simple way to access temperature data from various weather stations. You can expand its functionality by adding more endpoints or custom features.

- Users can modify the Flask application to adapt it to specific use cases or integrate it with other systems.

- The project's web interface provides users with API URL examples for quick access to the data they need.

- Remember to adjust the folder paths and data files as necessary to match your local setup.

Explore the world of weather data with the Weather API Builder, and utilize historical temperature information for various applications and research purposes.

Happy coding!
