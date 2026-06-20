# Applied Data Science Capstone Project: Predicting Falcon 9 First-Stage Landing Success

## Project Overview

This project focuses on predicting the successful landing of the SpaceX Falcon 9 first-stage booster. SpaceX has significantly reduced launch costs by reusing the first stage of its rockets, enabling launches at approximately $62 million compared to competitors whose costs often exceed $165 million. Accurately predicting landing outcomes provides valuable insights into launch economics and can help organizations estimate launch costs when competing with SpaceX for commercial launch contracts.

## Project Objectives

The project was completed through a series of interconnected modules that covered the full data science lifecycle, from data acquisition to machine learning model deployment.

### 1. Data Collection and Wrangling

* Retrieved historical Falcon 9 launch data through the SpaceX REST API.
* Extracted key launch parameters, including payload information, launch sites, booster details, and landing outcomes.
* Cleaned, transformed, and standardized the dataset to ensure consistency and data quality.
* Handled missing values and prepared the data for analysis.

### 2. Web Scraping Falcon 9 Launch Records

* Collected additional Falcon 9 launch records from Wikipedia using BeautifulSoup.
* Parsed HTML tables and converted the extracted information into structured Pandas DataFrames.
* Integrated scraped data with API-sourced datasets for comprehensive analysis.

### 3. Exploratory Data Analysis (EDA)

* Performed exploratory analysis to identify trends, patterns, and relationships among launch variables.
* Utilized Matplotlib and Seaborn to visualize launch outcomes, payload masses, launch sites, and orbital destinations.
* Generated training labels representing successful and unsuccessful booster landings.

### 4. Database Integration and SQL Analysis

* Loaded the processed dataset into a Db2 database.
* Executed SQL queries to answer business and operational questions related to launch performance.
* Leveraged SQL for efficient data exploration and validation.

### 5. Feature Engineering and Geographic Visualization

* Engineered predictive features from existing variables to improve model performance.
* Created interactive geographic visualizations using Folium.
* Analyzed launch site locations and landing success patterns through map-based visual analytics.

### 6. Interactive Dashboard Development

* Built an interactive dashboard using Plotly Dash.
* Implemented dynamic filters, dropdown menus, and range sliders for real-time data exploration.
* Developed interactive pie charts and scatter plots to enhance user-driven analysis.

### 7. Machine Learning Modeling and Optimization

* Standardized feature values and split the dataset into training and testing subsets.
* Developed and evaluated multiple classification models, including:

  * Logistic Regression
  * Support Vector Machine (SVM)
  * Decision Tree Classifier
  * K-Nearest Neighbors (KNN)
* Applied GridSearchCV for systematic hyperparameter tuning.
* Evaluated model performance using accuracy scores and confusion matrices.

## Results

| Model                        | Test Accuracy            |
| ---------------------------- | ------------------------ |
| Decision Tree Classifier     | 94.44%                   |
| Support Vector Machine (SVM) | 83.33%                   |
| K-Nearest Neighbors (KNN)    | 83.33%                   |
| Logistic Regression          | Evaluated for comparison |

The Decision Tree Classifier achieved the highest predictive performance, attaining an accuracy of **94.44%** on the test dataset.

## Key Insights

* Launch success rates improved over time as SpaceX gained operational experience.
* Payload mass, orbit type, launch site, and booster reuse characteristics were influential predictors of landing success.
* Feature engineering and hyperparameter optimization significantly improved model performance.
* Geographic and interactive visualizations provided valuable context for understanding launch outcomes.

## Conclusion

This project demonstrates a complete end-to-end data science workflow, encompassing data collection, cleaning, exploratory analysis, database querying, feature engineering, interactive visualization, and machine learning model development. The final predictive model successfully forecasts Falcon 9 first-stage landing outcomes with high accuracy, providing actionable insights into launch reliability and cost estimation. The findings highlight the effectiveness of data-driven approaches in supporting decision-making within the aerospace industry and competitive launch market.

## Acknowledgments

I would like to express my gratitude to the following organizations for their support and resources throughout this project:

* IBM – For designing and delivering the Applied Data Science Capstone course, as well as providing comprehensive learning materials and hands-on project guidance.
* Coursera – For offering an accessible and engaging platform through which the course content and practical exercises were delivered.
