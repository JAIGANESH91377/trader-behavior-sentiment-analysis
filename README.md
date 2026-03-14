# Trader Behavior vs Market Sentiment Analysis

This project analyzes how market sentiment (Fear & Greed Index) influences trader behavior and profitability. The analysis combines trading data with sentiment indicators to uncover patterns in trading activity, profitability, and risk-taking behavior.

---

## Objective

The goal of this project is to understand how traders react to different market sentiment conditions and identify behavioral patterns that influence trading performance.

---

## Dataset

Two datasets were used:

1. **Trader Data**
   - Trade execution details
   - Trade size
   - Closed profit/loss
   - Trade timestamps

2. **Market Sentiment Data**
   - Fear & Greed Index
   - Sentiment classification (Fear, Greed, Neutral, etc.)

The datasets were merged based on the **trading date**.

---

## Methodology

The analysis was performed using the following steps:

1. **Data Cleaning**
   - Handled datetime formats
   - Removed duplicates
   - Verified missing values

2. **Feature Engineering**
   - Daily trader metrics
   - Number of trades
   - Average trade size
   - Daily profitability
   - Long/short ratio

3. **Sentiment Analysis**
   - Compared trader profitability across sentiment categories
   - Examined trading activity patterns during Fear vs Greed markets

4. **Trader Segmentation**
   - Frequent vs Infrequent Traders
   - High Profit vs Low Profit Traders
   - High Risk vs Low Risk Traders

5. **Behavioral Clustering (Bonus)**
   - Applied KMeans clustering to identify trader archetypes
   - Features used:
     - Number of trades
     - Average trade size
     - Total profitability

---

## Key Insights

- Traders tend to generate **higher profits during Fear and Extreme Fear market conditions**, likely due to increased volatility.
- **Frequent traders show higher profit potential**, but also larger variability in performance.
- **High-risk traders exhibit greater profit dispersion**, indicating that larger trade sizes amplify both gains and losses.
- Greed-driven markets appear to produce **more stable but lower profitability**.

---

## Strategy Recommendations

Based on the analysis, several trading strategy adjustments can be considered:

- Increase trading activity during **fear-driven markets** where volatility is higher.
- Reduce position sizes during **extreme greed periods** to manage risk.
- Implement **adaptive risk management**, adjusting trade sizes depending on market sentiment.
- Use **volatility-based trading strategies** during uncertain market conditions.

---

## Bonus Analysis

An unsupervised clustering model was used to identify **trader behavioral archetypes**.

The clustering analysis revealed:

- Highly active traders with large profits
- Moderate traders with balanced performance
- Low-activity traders with smaller profit outcomes

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## How to Run

1. Clone this repository
git clone https://github.com/your-username/trader-behavior-sentiment-analysis.git


2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn


3. Run the notebook
jupyter notebook assignment.ipynb


---

## Author
Jaiganesh Mabbu
