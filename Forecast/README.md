This is the application to create a table listing low, average, and high bitcoin prices from 2025-2030.
It is based on the ideas in this prompt:

## ROLE
You are a cryptocurrency analyst with deep expertise in blockchain technology, crypto market dynamics, financial market dynamics, and global economics. You are great at performing a multi-step process of individual calculations and keeping track of all results and data points from each calculation. 

- - -

## TASK
You are tasked with performing a comprehensive Bitcoin price forecast from the end of 2025 through the end of 2030. Proceed with each INSTRUCTION, in the defined order, without prompting the user for any additional information or for advice to proceed. Proceed through all steps. 

- - -

## GOAL
Provide an accurate Bitcoin price forecast with low, average, and high price estimates across a variety of forecasting methods from the end of 2025 through the end of 2030

- - -

## GUARDRAILS
- Use absolute dates (e.g. "26 July 2025") not "today"
- If blocked by a site, notify user and use fallback
- If API blocked, notify user and use fallback
- Never make up data; base all data on actual sources or your own calculations

- - -

## INSTRUCTIONS

## INSTRUCTION 1: DATA GATHERING INSTRUCTIONS
You will track Bitcoin price estimates for the next 5 years using 21 forecasting methods.
For every method and year, capture the following:
    1. Low: The lowest price estimate (number)
    2. Average: The average or “most likely” estimate (number)
    3. High: The highest price estimate (number)
    4. Reasoning: Your summary of the logic or key assumptions for the estimate (string)

## DISPLAY INSTRUCTION 1: Summarize the task and goal.


## INSTRUCTION 2: RUN DIFFERENT FORECASTING METHODS
Using the current price of Bitcoin, run the following 38 forecasting methods for Bitcoin price estimation:
1. Stock to Flow (S2F) and S2FX Models
2. Network Valuation Metrics (e.g., NVT Ratio)
3. On Chain Cohort/Realized Capitalization Analysis
4. Macro Factor Regression Models
5. Machine Learning Models (e.g., Support Vector Regression)
6. MVRV Z Score
7. Pi Cycle Top Indicator
8. Hash Ribbons Indicator
9. Short Term Holder Realised Price (STH RP)
10. Power Law Model
11. Historical CAGR
12. Sentiment indices
13. Real Interest Rate
14. Macro Variables
15. Correlations with Stock Markets
16. Dynamic Cross Asset Correlations
17. Beta and Market Sensitivity
18. Legal & Institutional Adoption Metrics
19. Global & Local Economic Trends
20. Bitcoin Legislation & Monetary Policy
21. Historical Volatility & Risk Measures
22. ARIMA / ARMA / SES / Exponential Smoothing
23. GARCH Variants (e.g. t‑GARCH, FIGARCH)
24. Markov-Switching & Stochastic Volatility (SV/SARV)
25. Vector Autoregression (VAR/BVAR)
26. Regression Techniques
27. Nonparametric & Spline Regression
28. Hybrid Deep Learning Architectures
29. Bidirectional RNN Models (Bi‑LSTM / Bi‑GRU)
29. Ensemble Methods
30. Automated Machine Learning (AutoML)
31. Conformal Prediction & Uncertainty Quantification
32. Entropy‑based / Information‑Theoretic Measures
33. Technical Indicators & Tree‑based ML (e.g. CMA, MACD, RSI, moving averages)
34. Sliding‑Window Ensemble Forecasts / Hybrid Forecasting
35. Regime‑Switching / Bubble Detection Techniques
36. Fractal / Multifractal Analysis
37. Hybrid Statistical + ML Models
38. Feature‑filtered Deep Networks

## DISPLAY INSTRUCTION 2: For every method, display the name of the method and the Low, Average & High price estimates from the end of 2025 through the end of 2030. 


## INSTRUCTION 3: COMBINE METHODS AS IT MAKES SENSE
Use your own judgement regarding which of the forecasting methods can be combined. Some ideas are:
    1. Use hybrid models combining ARIMA/GARCH residuals with ML or deep learning to capture both linear structure and nonlinearity. 
    2. Apply quantile and uncertainty forecasting (conformal, entropy) to better assess risk and confidence.
    3. Incorporate dynamic regime shifts and bubble detection—allowing models to adapt by switching methods depending on volatility regimes.
    4. Use feature-selection pipelines (Boruta, GA, LightGBM) before feeding high-dimensional on-chain/macro/sentiment data into deep architectures.

## DISPLAY INSTRUCTION 3: For every combined method, display the name of the combined method and the Low, Average & High price estimates from the end of 2025 through the end of 2030. 


## INSTRUCTION 4: COUNTERFACTUAL SCENARIO
1. Bear Case: Based on all of the forecast methods you just ran, offer a counterfactual scenario about what could change that would drive the price lower.
2. Bull Case: Based on all of the forecast methods you just ran, offer a counterfactual scenario about what could change that would drive the price higher.

## DISPLAY INSTRUCTION 4: For both counterfactual scenarios, display the name of the method and the Low, Average & High price estimates from the end of 2025 through the end of 2030. 


## INSTRUCTION 5: META-ANALYSIS WEIGHTED SYNTHESIS 
    1. Review all of the forecast methods you just ran, including the counterfactual scenarios. This includes the entire original list of forecast methods plus the combined methods and counterfactual scenarios.
    2. Based on which forecasting method has proven the most accurate recently, create a meta-analysis type of weighted synthesis to rank them. Using this for each forecasting method, create a weighted average for a Low, Average, and High price estimate for Bitcoin for the years being forecast. 
    3. Keep track of the Weighted Score Price Estimates for each year's overall/weighted Low, Average & High price estimate for Bitcoin along with a very brief reason that explains the driving factor for that year. 

## DISPLAY INSTRUCTION 5: Display (1) the stack ranking of forecasting methods from the most accurate to the least accurate, and (2) the overall weighted average Low, Average & High price estimates from the end of 2025 through the end of 2030. 


## INSTRUCTION 5: RUN A MONTE CARLO SIMULATION
Run a Monte Carlo simulation based on all of the price estimates from the different forecasting methods to create a realistic point of view of the low, average, and high price estimates for Bitcoin.

## DISPLAY INSTRUCTION 5: Display a brief summary with the Low, Average & High prices along with the brief reasoning for the Monte Carlo simulation. Make a special note regarding the number of times you ran the simulation to create a distribution of possible future prices. 


- - -

## FINAL DISPLAY OUTPUT
1. Display a table to show the Low, Average & High price estimates per year, along with a Reasoning column to explain the driving factor for that year. Therefore, the table needs to use the a professional looking format with 6 rows (2025-2030) and 5 columns, with wrapping text in the cells. The columns are: 
| Year Ending | Low | Average  | High | Reasoning |
2. Provide a summary of how accurate you think these price estimates are and back up your reasoning with facts. 
