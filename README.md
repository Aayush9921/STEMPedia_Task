# STEMPedia Task 13

**We want to create the list of all CBSE and ICSE schools in India. How will you go about collecting this data? Share your methodology and the metrics you would like to capture for each school to understand the market better.**

According **Prokerala webpage, total 16950 CSEB school and 2050 ICSE schools.** But I Extract only 
**2910 schools in CBSE and 185 schools in ICSE schools.**I don't know why this happend.

# Extracting Data from Prokerala using BeautifulSoup

## Introduction
This project involves extracting data about CBSE and ICSE schools in India from the Prokerala website using Python's BeautifulSoup library. The goal is to collect and organize relevant data to better understand the school market in India.

## Methodology
To extract the data, the following steps were followed:

1. **Identify the Target Website**: The website used for data extraction is [Prokerala](https://www.prokerala.com/).
2. **Inspect the Website Structure**: The HTML structure of the school listings page was analyzed using browser developer tools to identify relevant tags and classes containing the required information.
3. **Setup Python Environment**: Python was used for web scraping, with the BeautifulSoup library for parsing HTML content.
4. **Send HTTP Requests**: The `requests` library was used to send GET requests to fetch the webpage content.
5. **Parse HTML Content**: BeautifulSoup was utilized to parse the HTML and extract the desired data by targeting specific tags and attributes.
6. **Store Data**: Extracted data was structured and stored in a tabular format (e.g., CSV) for further analysis.

## Metrics Captured
The following metrics were collected for each school:

- **School Name**: The official name of the school.
- **Address**: The full address, including city, state, and pin code.
- **Phone Number**: Contact number(s) of the school.
- **Affiliation**: Whether the school is affiliated with CBSE or ICSE.

## Technologies Used
- **Python**: Programming language for web scraping.
- **BeautifulSoup**: Library for parsing and navigating HTML.
- **Requests**: Library for sending HTTP requests.
- **Pandas**: For organizing and storing extracted data in a structured format.

## How to Run
1. Clone the repository to your local machine.
2. Install the required libraries using:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the script to start the data extraction process:
   ```bash
   python extract_schools.py
   ```
4. The extracted data will be saved in a file named `CBSC_DATA.csv` and `ICSC_DATA.csv`.

## Future Work
- Automate the scraping process to handle pagination and dynamically loaded content.
- Add more metrics such as email addresses, website URLs, and the number of students.
- Perform exploratory data analysis on the extracted data to identify trends and insights.

## Disclaimer
This project is for Assesment in STEMPedia, practice and understand purposes only. Ensure compliance with the website's terms of service before scraping data.



