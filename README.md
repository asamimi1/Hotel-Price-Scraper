# Hotel Price Scraper

This is a Python script that scrapes hotel prices from [hotels.com](https://www.hotels.com) based on location and dates provided. It uses Selenium to automate interactions with the website, extracting relevant information such as hotel name, location, price, and rating, and saving the data in an Excel file.

## Getting Started

1. Clone this repository to your local machine:

    ```bash
    git clone <repository-url>
    ```

2. Navigate to the project directory:

    ```bash
    cd hotel-price-scraper
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Make changes in the `config.py` file:

    - Set the `LOCATION`, `CHECK_IN_DATE`, and `CHECK_OUT_DATE` variables to specify the location and dates for which you want to scrape hotel prices.

5. Ensure that you have [Chrome](https://www.google.com/chrome/) installed on your machine. Additionally, download the appropriate [ChromeDriver](https://chromedriver.chromium.org/) compatible with your Chrome version and operating system. Place the ChromeDriver executable in the project directory.

6. Run the script from `main.py`:

    ```bash
    python main.py
    ```

7. Once the script finishes running, you will find the scraped hotel data saved in the `hotel_data.xlsx` file.

## Configuration

Make sure to update the following variables in the `config.py` file before running the script:

- `LOCATION`: The location for which you want to search for hotels.
- `CHECK_IN_DATE`: The check-in date for your hotel stay (format: "MM-DD-YYYY").
- `CHECK_OUT_DATE`: The check-out date for your hotel stay (format: "MM-DD-YYYY").

## Dependencies

- [Selenium](https://pypi.org/project/selenium/): Web scraping library for Python.
- [openpyxl](https://pypi.org/project/openpyxl/): Library for reading and writing Excel files.
