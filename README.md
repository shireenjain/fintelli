# Fintelli: A Quantitative Financial Advisor

**Team Members**:
- Shireen Jain
- Amodh Sharma
- Shruti Gupta
- Ananya Prasad
- Harshita Saini

---

### Introduction and Project Novelty

- **Objective**:  
  The goal of this project is to implement and evaluate diverse quantitative investment strategies within the context of the Indian stock market, specifically using the Nifty 50 and Nifty 500 indices.  
  This will contribute to the development of a **quantitative advisor chatbot** designed to assist investors in making informed decisions. The chatbot will provide tailored investment advice based on quantitative data.

- **Key Components**:  
  The project, in its current stage, explores three distinct quantitative investment strategies. Sample outputs and datasets are provided in a Google Sheet, which can be accessed [here](https://docs.google.com/spreadsheets/d/1yUuq0K5O5NqUBcGugn1IqANLC-laJqKY6tpvO0AOHmg/edit?usp=sharing). The trading strategies are:

  - **Equal-Weight Nifty 50 Index Fund**:  
    - **Objective**: Challenge the traditional market-capitalization-weighted approach by allocating equal weight to all stocks in the Nifty 500 index.  
    - **Strategy**: Promotes a more balanced risk distribution across the portfolio.

  - **Quantitative Momentum Investing**:  
    - **Objective**: Identify and invest in Nifty 50 stocks exhibiting strong recent performance.  
    - **Approach**:  
      - Analyze historical price trends across multiple timeframes (1 year, 6 months, 3 months, and 1 month).  
      - Rank stocks based on percentile scores of returns.  
      - Use a High Quality Momentum (HQM) score to combine these rankings.

  - **Quantitative Value Investing**:  
    - **Objective**: Identify undervalued Nifty 50 stocks with strong growth potential.  
    - **Approach**:  
      - Analyze key financial ratios like P/E, P/B, and price-to-sales.  
      - Apply filters and thresholds to select undervalued stocks.  
      - Compute a Robust Value (RV) score by aggregating percentiles of these ratios.

- **Integration**:  
  - These strategies will form the foundation of an advisor chatbot that equips investors for making investment decisions.  
  - The chatbot will also be incorporating company research, data trends, and financial metrics to offer a comprehensive and diverse approach to investing.

- **Innovation and Diversity**:  
  - The project offers a diverse set of investment strategies to cater to different investor profiles, enhancing decision-making through:
    - Portfolio balance (Equal-Weight Strategy).
    - Momentum-based performance (Momentum Strategy).
    - Value-based stock selection (Value Strategy).

- **End Goal**:  
  - To provide a holistic and customizable investment experience, integrating multiple investing strategies and real-time data from the Indian stock market.

---
