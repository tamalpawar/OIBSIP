# Level 2 — Task 4: Unveiling the Android App Market

## Google Play Store Analysis

### Project Overview

This project analyzes the Google Play Store ecosystem using data analysis and visualization techniques.

The analysis focuses on app categories, ratings, reviews, installs, app size, pricing, and user review sentiment to identify meaningful patterns and insights.

### Objectives

- Clean and preprocess Google Play Store data
- Analyze app categories and app distribution
- Study app ratings and category-wise ratings
- Analyze the relationship between app size and installs
- Compare free and paid applications
- Analyze paid app pricing
- Estimate revenue by category
- Perform sentiment analysis on user reviews
- Generate data-driven insights for app developers

### Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- TextBlob / VADER
- Plotly
- Jupyter

### Dataset

The project uses the Google Play Store Apps dataset along with the Google Play Store User Reviews dataset.

The datasets contain information about:

- App name
- Category
- Rating
- Reviews
- Size
- Installs
- Type
- Price
- Content Rating
- Genres
- User Reviews
- Sentiment

### Data Cleaning

The dataset was cleaned by:

- Removing duplicate records
- Handling missing values
- Correcting invalid rating records
- Converting reviews and installs into numeric values
- Converting app size into MB
- Converting prices into numeric values
- Handling missing categorical/version values
- Preparing user reviews for sentiment analysis

### Analysis Performed

#### 1. Category Analysis

Analyzed the distribution of apps across categories and identified the most saturated categories.

#### 2. Ratings Analysis

Analyzed the overall rating distribution and calculated average ratings for each app category.

#### 3. Size vs Installs

Studied the relationship between application size and number of installs.

The correlation between app size and installs was approximately **0.169**, indicating a weak positive relationship.

#### 4. Pricing Analysis

Compared free and paid applications and analyzed the price distribution of paid apps.

Approximately **92.62%** of the analyzed apps were free, while **7.38%** were paid.

#### 5. Revenue Estimation

Estimated potential revenue for paid applications using:

`Estimated Revenue = Price × Installs`

This is an estimate because the dataset provides install ranges rather than exact installation counts.

#### 6. Sentiment Analysis

Analyzed user reviews and classified them into:

- Positive
- Negative
- Neutral

Sentiment was also analyzed across different app categories.

### Key Insights

1. **Highly competitive categories:** FAMILY is the most saturated category, followed by GAME and TOOLS. Developers entering these categories should focus on differentiation and usability.

2. **Negative feedback in Games and Social apps:** GAME has the highest negative sentiment share at approximately **37.20%**, followed by SOCIAL at **28.21%**.

3. **Free apps dominate:** Approximately **92.62%** of analyzed apps are free, suggesting that free or freemium models are common in the Google Play Store ecosystem.

4. **App size is not a strong driver of installs:** The size-install correlation of approximately **0.169** indicates that app size alone does not strongly determine download volume.

### Project Outputs

The `outputs/` folder contains visualizations for:

- Category distribution
- Top 10 category saturation
- Rating distribution
- Average rating by category
- Size vs installs
- Free vs paid applications
- Paid app price distribution
- Revenue by category
- Overall sentiment distribution
- Sentiment by category
- Interactive average rating visualization

### Conclusion

The analysis shows that the Google Play Store is highly competitive, with a large concentration of applications in a few major categories. Free applications dominate the ecosystem, while user sentiment varies significantly across categories.

For developers, differentiation, user experience, pricing strategy, and addressing user feedback are important factors when developing and positioning an application.