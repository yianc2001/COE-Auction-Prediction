# Cup of Exellence Auction Price Prediction
Final project of course **Statistical Learning and Deep Learning**(2023 Fall), National Taiwan University.

Contributers: 陳怡安 Yi-An Chen、林品柔 Pin-Jou Lin、簡言芳 Yen-Fang Chiang、黃泓愷 Hung-Kai Huang

# Table of Content
- [Introduction](#introduction)
- [Data](#data)
  - [Data Collection](#data-collection)
  - [Data Preprocessing](#data-preprocessing)
- [Descriptive Statistics](#descriptive-statistics)
- [Feature Selection](#feature-selection)
- [Models](#model)
- [Results](#results)
- [Take Away](#take-away)

# Introduction
# Data
Data source: website of [Alliance of Coffee Exellence](https://allianceforcoffeeexcellence.org/competition-auction-results/)
## Data Collection
Data was collected via web scraping, targeting specific pages that provide detailed records of coffee competitions. The extracted data includes:

- Ranking and Scores: Each coffee's competition rank and score.
- Origins and Estates: Details about the coffee's origin and the estate where it was grown.
- Variety and Processing Methods: Information about coffee varieties and their processing techniques.
- Flavor Notes: Descriptions of the coffee's aroma and flavor characteristics.
- Bidders: Information about the bidders, including bid amounts and winning companies.

  

## Data Preprocessing
To ensure the dataset's usability, the preprocessing steps included:

1. Structuring the extracted data into a tabular format.
2. Dealing with inconsistent data format, such as ranking and units of price.
3. Renaming columns for consistency and clarity (e.g., "Other" was renamed to "Coffee Characteristics").
4. Filling missing data with placeholders (e.g., "NaN") where applicable.
5. **Defining flavor metrics:** categorizing different flavor notes into specific characteristics.
   - Columns such as Coffee_characteristics, Flavor, and Acidity were cleaned by converting text to lowercase and removing unwanted characters like numbers and special symbols.
   - Key flavor and aroma descriptors (e.g., "clean," "balanced," "creamy") were identified and used to create binary features indicating the presence of these descriptors.
   - Flavor profiles were categorized into distinct groups such as "Roasted Flavor," "Spices Flavor," "Nutty/Cocoa Flavor," "Sweet Flavor," "Floral Flavor," "Fruity Flavor," and "Green Vegetative Flavor." This was achieved by matching text patterns in the Coffee_characteristics and Flavor columns.
   - Acidity was divided into specific types (e.g., "Malic," "Citric," "Tartaric") using a similar pattern-matching approach.
   - Binary and count-based features were added for each identified flavor and acidity characteristic, enriching the dataset for detailed analysis.

   
# Descriptive Statistics
# Feature Selection
# Models
# Results
# Take Away
# Presenation Slides
This is the [slides](https://github.com/yianc2001/COE-Auction-Prediction/blob/main/SLDL%20final.pdf) of our presentation.


