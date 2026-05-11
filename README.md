# Sentiment_Analysis_Time_Series
An end-to-end Exploratory Data Analysis (EDA) and interactive Power BI dashboard tracking temporal sentiment trends, customer engagement dynamics, and aspect-level brand health across 5 major smartphone manufacturers using 10,000+ social media records.

# EmotionEdge: Power BI Sentinel for Sentiment & Time-Series Intelligence
In today’s hyper-competitive smartphone market, product success depends entirely on user experience. **EmotionEdge** is an advanced analytics solution designed to transform raw, noisy feedback from 10,000+ multi-platform social media posts into actionable, real-time product intelligence. By employing **Exploratory Data Analysis (EDA)** in Power BI, this project extracts multidimensional customer sentiment, measures engagement patterns (likes, shares, comments), and tracks how customer feelings evolve over time across **8 critical hardware/software aspects**.

## ⚡ Key Visualizations & Dashboard Architecture
The final interactive dashboard acts as a strategic command center divided into:

1. **Brand Features vs. Sentiment Scores**: A heat map grid highlighting exactly where brands succeed or struggle (e.g., Apple's display vulnerabilities vs. Samsung's fast-charging strengths).
2. **Temporal Sentiment Trends (15-Month Timeline)**: A time-series stacked line chart tracing brand perception trajectories from January 2025 to March 2026.
3. **Sentiment-Engagement Relationship (Regression Plot)**: A scatter plot tracking the correlation between raw sentiment scoring (-1.0 to +1.0) and high-impact social media engagement (likes/shares).
4. **Cross-Platform Distributions**: A 100% stacked bar chart revealing how feedback tone differs across YouTube, Reddit, Instagram, Twitter, and Facebook.

## 🔍 Core Insights & Data Discovery

* **The Silent Majority vs. Vocal Minority**: High-engagement posts (higher likes and shares) skew heavily negative, proving that dissatisfied customers speak loudest on public forums.
* **Temporal Volatility**: Traced a sudden drop in **Google’s Performance sentiment** in early March 2026—an immediate early warning for product engineering.
* **Feature Drivers**: **Battery Life** and **Software/OS** updates show the strongest overall correlation with the composite Sentiment Index, identifying them as key customer retention drivers.
* **Competitive Positions**: Samsung leads heavily in Charging Speed but lags consistently in Software/OS. Xiaomi remains the undisputed leader in price-driven positive sentiment.

## 🛠️ Prerequisites & Technical Stack

### Software & Tools Required
* **Power BI Desktop** (to run, filter, and interact with the `.pbix` file)
* **Power BI Service** (for cloud publishing and sharing)
* **Microsoft Excel / Python (Pandas)** (for initial raw data profiling)

### Skills Applied
* **DAX (Data Analysis Expressions)**: Created custom measures for time intelligence, rolling averages, and engagement-weighted composite sentiment scores.
* **Power Query Editor**: Conducted data cleansing, column formatting (Excel serial dates to standard datetime), and merging 4 separate datasets into 1 consolidated model.
* **Data Modeling**: Built relationships between user metrics, aspect attributes, and chronological dimensions.

## 📊 Dataset Schema
The project uses `mobile_brand_sentiment_dataset.xlsx`, containing **10,000 records** spanning 15 months (Jan 2025 – Mar 2026):

* **Brand**: Smartphone brand (Apple, Samsung, Google, Xiaomi, OnePlus).
* **Platform**: Social media source (Instagram, Twitter, YouTube, Reddit, Facebook).
* **Date**: Timestamp of post creation.
* **Topic**: Feature-level aspect (Battery, Camera, Performance, OS, Price, Display, Build, Charging).
* **Sentiment**: Categorical label (Positive / Neutral / Negative).
* **Sentiment Score**: Numeric range from `-1.0` (Highly Negative) to `+1.0` (Highly Positive).
* **Engagement Metrics**: Raw counts of Likes, Shares, and Comments used to calculate weighted indices.
* **Text**: Raw user review comment text (utilized for tooltips and underlying analysis).

## 📈 Strategic Business Recommendations

* **Targeted Marketing**: Direct marketing teams to execute feature-specific campaigns to counteract negative brand perceptions (e.g., highlighting Samsung's UI/OS improvements).
* **Rapid-Response QA**: Establish weekly product team reviews of the **Temporal Explorer** to detect software bug escalations immediately after public releases.
* **Executive Monitoring**: Integrate the composite **Sentiment Index (0-100)** as a primary monthly KPI for senior leadership.
