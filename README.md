# Jumia Web Scraper

This project is a web scraping tool that extracts Flash Sales(Live Now) product information from the Jumia Online Shop (Kenya). The scraper collects details like product names, prices, stock availability, ratings, and images. The data is then stored in a CSV file and can be analyzed using Jupyter Notebooks.

## Project Structure

The project contains the following structure:

```
Jumia Web Scraper/
│
├── venv/                         # Virtual environment for package dependencies
├── Jumia Web Scraper.ipynb        # Jupyter Notebook for web scraping logic
├── jumia_products.csv            # CSV file where the extracted product data is saved
├── Jumia Data Analysis.ipynb     # Jupyter Notebook for data analysis and visualization
└── README.md                     # Project description and guide
```

### 1. **Virtual Environment (venv)**
   The project uses a Python virtual environment to manage dependencies. It includes the following libraries for web scraping, data manipulation, and analysis, including:
   - `requests`
   - `beautifulsoup4`
   - `pandas`
   
   You can create the virtual environment by running:
   ```bash
   python -m venv venv
   ```

   After activation, install the required packages with:
   ```bash
   pip install -r requirements.txt
   ```

### 2. **Jumia Web Scraper.ipynb**
   This Jupyter Notebook contains the main code for scraping product details from the Jumia website. It sends requests to Jumia, extracts relevant product data (name, price, discount, stock availability, etc.), and stores the results in a CSV file (`jumia_products.csv`).

   **Key functionalities:**
   - Scrapes multiple pages of products.
   - Collects data such as product name, price, discount, rating, and stock availability.
   - Saves the extracted data to a CSV file (`jumia_products.csv`).

### 3. **jumia_products.csv**
   This CSV file stores the extracted product details. The columns include:
   - Product Name
   - Price
   - Original Price
   - Discount
   - Stock Availability
   - Image URL
   - Rating
   - Product Link

   This file is updated with the latest product data after each scraping run.

### 4. **Jumia Data Analysis.ipynb**
   This Jupyter Notebook is designed for analyzing and visualizing the data collected in `jumia_products.csv`. The analysis includes:
   - Summary statistics
   - Visualizations (e.g., bar charts, histograms) of product prices, ratings, and stock availability.
   - Insights into the most popular products, best discounts, and other trends.
     ***Data analysis is still ongoing...***

## Getting Started

### Prerequisites

1. **Python**: Ensure that Python 3.12 or later is installed on your machine.
2. **Virtual Environment**: You can create and activate a virtual environment as shown above.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/jumia-web-scraper.git
   cd jumia-web-scraper
   ```

2. Create and activate the virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Scraper

1. Open the `Jumia Web Scraper.ipynb` notebook in Jupyter and run the cells to scrape product data from Jumia.
2. The results will be saved in the `jumia_products.csv` file.

### Running Data Analysis

1. Open the `Jumia Data Analysis.ipynb` notebook in Jupyter.
2. Load the `jumia_products.csv` file to begin analyzing the scraped data.
3. Explore visualizations and insights based on the product data.

## Project Overview

The Jumia Web Scraper is a simple yet powerful tool to collect product data from the Jumia Online Shop (Kenya). The scraper is designed to extract key product information such as product names, prices, stock availability, and ratings.

After gathering the data, it can be analyzed using the `Jumia Data Analysis.ipynb` notebook, which provides valuable insights and visualizations to help understand trends in the Jumia marketplace.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

### Adding the README file to your repository

1. Create a file named `README.md` in your project folder.
2. Paste the above content into the file and save it.
3. Commit and push the `README.md` file to your GitHub repository:

```bash
git add README.md
git commit -m "Add README file"
git push origin main
```

This `README.md` file will provide your repository visitors with all the necessary information to understand, set up, and use your Jumia Web Scraper project.
