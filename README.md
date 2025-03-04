# nigeria-weather-scraper-api

Project Overview
The Weather Scraper API is a FastAPI-based web service that scrapes weather data for Nigerian states (Abeokuta, Bauchi and Benin City). It processes the data and then writes it to a Google sheet using gspread. The API also provide a GET endpoint that retrieves the latest stored weather data.

⚡Features
FastAPI Endpoint: Exposes a GET endpoint (/weather) to fetch the latest weather data.
Extracts weather data using BeautifulSoup.
Google Sheets Integration: Writes scraped data to a Google Sheet using gspread.
Dependency Management: Uses poetry for managing dependencies.
Testing: Includes test cases with pytest.
Uses virtual environment for an isolated python environment.
🛠️ Installation & Setup
1. Clone the Repository
git clone https://github.com/DarkKnight845/Weather-API-Ng
2. Set Up Virtual Environment
python -m venv venv
source venv/bin/activate # For Linux/macOS
venv\Scripts\activate # For Windows
3. Install Dependencies with Poetry
poetry install package
4. Set Up Google Sheets Credentials
Create a Service account on Google Cloud Console.
Download the JSON credentials file.
Save it as service_account inside the project directory.
Share the Google Sheet with the service account email.
🚀 Running the API
Start the FastAPI Server
poetry uvicorn main:app --reload

Test the API via Swagger UI


 Running Tests
To run tests using pytest:

pytest
🧑‍🤝‍🧑 Dependencies
FastAPI
BeautifulSoup
Requests
Gspread
Pytest
