# Python-Aviation-Accident-Analysis-

## Overview

This project focuses on analyzing aviation accident data to uncover insights and trends that can enhance safety and operational efficiency in the aviation industry. By utilizing statistical methods and data visualization, we aim to provide a comprehensive understanding of the factors contributing to aviation accidents.

## Project Goal

The primary goal of this project is to analyze aviation accident data to identify key trends, risk factors, and safety improvements. This analysis will support decision-making for stakeholders in the aviation industry, including regulatory agencies, airlines, and safety organizations.

## Benefits to the Industry

- **Enhanced Safety**: By identifying common factors in aviation accidents, stakeholders can implement preventive measures.
- **Informed Decision-Making**: Data-driven insights can guide policy changes and operational improvements.
- **Public Awareness**: Increased understanding of aviation safety issues can help inform the public and improve trust in air travel.

## Dataset

The dataset includes the following key columns related to aviation accidents:

- **Event.Id**: Unique identifier for the event.
- **Accident.Number**: Unique accident number.
- **Event.Date**: Date of the accident.
- **Location**: Geographic location of the accident.
- **Country**: Country where the accident occurred.
- **Injury.Severity**: Severity of injuries (e.g., non fatal, minor, serious, fatal, uninjured).
- **Make**: Manufacturer of the aircraft.
- **Model**: Model of the aircraft.
- **Total.Fatal.Injuries**: Total number of fatal injuries.
- **Weather.Condition**: Weather conditions at the time of the accident.
- **year**: Year of the accident.
- **City**: City where the accident occurred.

The full dataset is included in this repository.

## Data Extraction

An attempt was made to extract aviation accident causes data using the Wikipedia API. The aviation accident data was obtained from a Kaggle dataset. As a beginner, the data cleaning process may not have been perfect, and users should exercise caution when interpreting the results. Further investigation is encouraged before making any decisions based on the findings. 

## Python Libraries Used

This project utilizes the following Python libraries:

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For static data visualization.
- **Seaborn**: For statistical data visualization.
- **Plotly**: For interactive visualizations.
- **SciPy**: For statistical analysis.
- **Requests**: For API data retrieval.
- **BeautifulSoup**: For parsing HTML and XML documents (used in conjunction with API data extraction).
- **Pyspan**: For cleaning and processing data.

## Target Audience

This project is intended for:

- **Aviation Industry Professionals**: Including safety analysts, regulators, and airline operators.
- **Data Analysts**: Interested in aviation safety and incident analysis.
- **Researchers**: Focusing on transportation safety and related fields.
- **General Public**: Anyone interested in understanding aviation safety trends.

## Disclaimer

This analysis is based on available data and may not reflect accurate or reliable conclusions. Users should exercise caution when interpreting the results. The analysis should not be taken as definitive, and further investigation is encouraged before making any decisions based on the findings.

## Getting Started

### Prerequisites

You need a Google account to access Google Colab.

### Opening the Notebook

1. Open the Google Colab notebook:
   - Open the provided Google Colab notebook file 'Python_Aviation_Accident_Analysis.ipynb` in this repository..

2. Load the dataset:
   - The dataset is included in the repository.

### Installation

To install the necessary libraries, run the following command:

```
pip install pandas numpy matplotlib seaborn plotly scipy requests beautifulsoup4 pyspan
```
### Usage

Here’s an example of how to import the libraries and load your dataset:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
from bs4 import BeautifulSoup
import requests
import pyspan as ps
```
# Load your dataset
path = '/content/AviationData.csv'
df = pd.read_csv(path, encoding='ISO-8859-1')

### Running the Analysis

You can run your analysis with the following code:

```python
# Example analysis code
summary = df['Total.Fatal.Injuries'].describe()
print("Summary of Total Fatal Injuries:", summary)
```

## Analysis Ideas

- **Descriptive Statistics**: Analyze basic statistics for numerical columns.
- **Injury Severity Analysis**: Explore the distribution of injury severity.
- **Weather Conditions**: Investigate how weather affects accident severity.
- **Accidents Over Time**: Plot the number of accidents per year.
- **Aircraft Category Analysis**: Examine the relationship between aircraft category and injury severity.
- **Geographical Analysis**: Visualize the distribution of accidents by country.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

## License

This project is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. See the [LICENSE](LICENSE) file for details.

## Contact

For inquiries or feedback, please reach out to mehreen.aman@gmail.com.
