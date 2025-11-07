🛫 Flight Price Prediction – Data Preprocessing & Feature Engineering

This project involves cleaning, exploring, and encoding a flight price dataset to prepare it for machine learning model training. The dataset contains information about various domestic airlines, flight details, timing, stops, and ticket prices.

📊 Dataset Overview

The cleaned dataset contains 300,153 rows and 12 columns.
Each record represents a flight along with its associated features and price.

Features Explained:

Airline: Name of the airline (6 unique airlines).

Flight: Flight code (categorical).

Source City: City of departure (6 unique cities).

Departure Time: Time of departure categorized into 6 bins.

Stops: Number of stops — encoded using Ordinal Encoding (zero, one, two_or_more).

Arrival Time: Time of arrival categorized into 6 bins.

Destination City: City of arrival (6 unique cities).

Class: Type of seat — Economy or Business.

Duration: Total travel time (in hours).

Days Left: Days remaining between booking and travel date.

Price: Ticket price (target variable).

🧹 Data Cleaning

Checked for missing values → No null entries found.

Verified data types for each column.

Inspected categorical and numerical distributions using .info() and .describe().

🔢 Feature Encoding

Ordinal Encoding applied on stops feature.

One-Hot Encoding applied on airline, source_city, and destination_city features to convert them into numerical format.

Generated 18 encoded columns representing categorical variables.

📈 Tools & Libraries Used

pandas for data manipulation

numpy for numerical operations

matplotlib & seaborn for data visualization

sklearn.preprocessing for encoding categorical features

📁 Output

After encoding, the dataset is ready for:

Exploratory Data Analysis (EDA)

Model training (e.g., regression models for price prediction)

🧠 Next Steps

Perform feature scaling and outlier detection.

Build and evaluate machine learning models (e.g., Linear Regression, Random Forest, XGBoost).

Optimize hyperparameters for better prediction accuracy.
