# Web Scraping Top 50 Movies

This project demonstrates how to scrape the top 50 movies by rank, title, and year from a web page, save the data into a CSV file, and also store it in an SQLite database. The project is implemented in Python and can be run in a Google Colab environment.

## Features
- Scrapes movie data from a provided URL.
- Saves the data into a CSV file.
- Stores the data in an SQLite database for easy querying.

## Prerequisites
Ensure you have the following installed:
- Python 3.x
- Required Python libraries: `pandas`, `beautifulsoup4`

You can install the required libraries using the following commands:

```bash
pip install pandas beautifulsoup4
```

## Files
- `webscraping_movies.ipynb`: Jupyter Notebook containing the project code.
- `Movies.db`: SQLite database file containing the scraped data.
- `top_50_films.csv`: CSV file containing the scraped data.

## Setup
### Step 1: Clone the repository
```bash
git clone <repository-url>
cd <repository-folder>
```

### Step 2: Run the Notebook
Open the `webscraping_movies.ipynb` notebook in Google Colab or any Jupyter Notebook environment and execute the code cells sequentially.

## How It Works
### 1. Import Required Libraries
The script uses the following libraries:
- `requests` for fetching the web page.
- `pandas` for handling and manipulating the data.
- `BeautifulSoup` from `bs4` for parsing the HTML.
- `sqlite3` for storing the data in an SQLite database.

### 2. Initialize Variables
- **URL**: Web page URL to scrape data from.
- **CSV File**: Path to save the scraped data in CSV format.
- **SQLite Database**: Name of the SQLite database file.

### 3. Scrape Data
- Fetch the HTML content using `requests`.
- Parse the HTML using `BeautifulSoup`.
- Identify and extract data from the relevant table on the web page.
- Store the data in a `pandas` DataFrame.

### 4. Save Data
- Save the DataFrame to a CSV file.
- Store the DataFrame into an SQLite database.

### 5. Output
The script produces the following outputs:
- A `top_50_films.csv` file containing the scraped movie data.
- An SQLite database file (`Movies.db`) containing the same data in a table named `Top_50`.

## Usage
### Run the Python Script
You can execute the script directly in a terminal or in a notebook environment.

For terminal:
```bash
python3 webscraping_movies.py
```

For Jupyter Notebook, execute each code cell sequentially.

## Example Output
**CSV Output:**
| Average Rank | Film               | Year |
|--------------|--------------------|------|
| 1            | The Shawshank Redemption | 1994 |
| 2            | The Godfather      | 1972 |
| ...          | ...                | ...  |

## Author
This project was developed as part of a hands-on lab exercise.

## License
This project is open-source and available under the MIT License.
