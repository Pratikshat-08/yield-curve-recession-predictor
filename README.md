# yield-curve-early-warning-system
Yield curve inversion as a recession signal: a quantitative framework for macro risk forecasting using the 10Y–2Y spread and logistic regression.


# Project Purpose
This repository provides a reproducible analysis of whether yield curve inversions (10Y–2Y spread turning negative) serve as reliable leading indicators of U.S. recessions.

# Abstract
This study examines the relationship between the U.S. Treasury 10-Year minus 2-Year yield spread (T10Y2Y) and subsequent economic recessions using 600 monthly observations spanning 1976 to 2025. Employing descriptive statistics, logistic regression modelling, and recession lead-time estimation, the analysis evaluates whether yield curve inversions serve as reliable leading indicators of economic downturns. Results confirm a strong negative relationship between the yield spread and future recession probability, with inversions preceding recessions by an average of 11 months.


# Introduction
The shape of the yield curve specifically the spread between long-term and short-term Treasury yields has long been regarded as one of the most closely monitored forward-looking indicators of macroeconomic conditions. Under normal circumstances, a positively sloped yield curve reflects expectations of sustained economic growth and positive inflation. When this relationship reverses and short-term rates rise above long-term rates, the resulting inversion has historically preceded the majority of major U.S. recessions.
This study investigates the empirical relationship between the 10Y–2Y Treasury yield spread and the subsequent occurrence of recession, using monthly data sourced from the Federal Reserve Economic Data (FRED) database. The findings are evaluated in the context of Treasury management and ALM, where yield curve dynamics directly inform funding strategy, interest-rate risk positioning, and liquidity planning.


# Methodology
Collected monthly 10-Year Treasury Yield and 2-Year Treasury Yield data from the Federal Reserve Economic Data (FRED) database for the period 1976–2025.

Calculated the 10Y–2Y yield spread.

Obtained U.S. recession data from the National Bureau of Economic Research (NBER) recession indicator series available through FRED.

Conducted descriptive statistical analysis to examine the distribution, variability, and key characteristics of the yield spread.

Identified yield curve inversion periods where the spread became negative and measured their frequency within the sample.

Analyzed extreme observations, including the deepest inversion and steepest positive yield curve, and linked them to historical economic conditions.

Compared average yield spreads during periods that were followed by a recession within the next 12 months against periods that were not.

Developed a logistic regression model with the yield spread as the independent variable and the occurrence of a recession within the subsequent 12 months as the dependent variable.

Estimated recession probabilities based on the logistic regression results and evaluated the relationship between yield curve movements and future economic downturns.

Performed lead-time analysis by measuring the time gap between the onset of yield curve inversions and the start of subsequent recessions.


# Analysis
Descriptive Statistics-
Analysis of the 10Y–2Y Treasury yield spread revealed that the series averaged 0.85 PP over the sample period, indicating that the yield curve remained positively sloped under normal economic conditions. However, the spread exhibited considerable variability, with a standard deviation of 0.91 PP, reflecting the changes in yield curve shape that occur across different economic conditions.
The spread ranged from a minimum of −2.14 PP observed during a period of severe inversion and acute economic stress to a maximum of +2.83 percentage points during a strong post-crisis recovery. Collectively, these statistics confirm that the yield curve varied substantially in shape across the sample period, consistent with its role as an indicator of evolving economic and monetary conditions.

Yield Curve Inversion Analysis-
Yield curve inversions defined as periods in which the 10Y–2Y spread was negative were observed in approximately 16.5% of all monthly observations, equating to roughly 99 months across the sample. Although inversions were relatively infrequent, but occurred mainly during specific economic stress periods, not randomly.
Yield curve inversions mainly occurred during times of economic uncertainty and tight monetary policy, showing they can act as an early warning sign of economic slowdown. A normal yield curve shows expectations of economic growth, while an inverted yield curve occurs when higher short-term rates signal slower future growth and increased recession risk. While the yield curve remained positively sloped for 83.5% of the sample, inversion episodes consistently preceded major economic downturns reinforcing their practical value as an early-warning signal.

Extreme Observations-
Deepest Inversion-March 1980
The strongest yield curve inversion happened in March 1980, when the 10Y–2Y spread fell to −2.14 percentage points. Short-term interest rates surged sharply above long-term rates, producing one of the most severe yield curve inversions in modern U.S. economic history. A deeper yield curve inversion may indicate not only a higher chance of recession but also how severe the economic stress could be, helping risk managers plan stress-test scenarios.

Steepest Yield Curve-February 2010
The steepest yield curve in the sample was recorded in February 2010, when the 10Y–2Y spread widened to +2.83 percentage points. This observation occurred approximately eight months after the official end of the Global Financial Crisis recession in June 2009.The very steep yield curve occurred because the Federal Reserve kept short-term interest rates near zero, while investors expected economic recovery and higher inflation in the future.
A direct comparison of these two extremes presents a compelling empirical narrative: the deepest inversion (−2.14 pp) coincided with peak recessionary stress under restrictive monetary policy, while the steepest positive spread (+2.83 pp) reflected recovery expectations under highly accommodative conditions. These contrasting observations demonstrate that the yield curve not only signals potential downturns through inversion, but also reflects improving economic conditions through steepening.

Recession vs. Non-Recession Period Comparison-
A comparison of yield spreads shows that periods preceding a recession had an average spread close to zero or slightly negative, while non-recession periods recorded a higher positive spread (+0.95), reinforcing the yield curve’s effectiveness as a predictor of future economic conditions.

Logistic Regression Model-
To measure how well the yield spread predicts future recessions, a logistic regression model was used, where the yield spread served as the predictor and whether a recession occurred within the next 12 months was the outcome variable. The estimated coefficient on the yield spread was −1.429, confirming a negative and economically meaningful relationship: as the spread declines, the probability of recession within the following 12 months increases significantly. This finding is consistent with the theoretical expectation that a flattening or inverting yield curve reflects tightening financial conditions and deteriorating growth expectations both of which are empirically associated with economic contraction. The model assigned its highest recession probability of 81.2% to March 1980, the period of the deepest inversion and a confirmed recession. Conversely, the lowest probability of 0.36% was assigned to February 2010, the period of the steepest yield curve and strongest post-crisis recovery expectations. 

Recession Lead-Time Analysis-
To assess the practical early-warning capability of yield curve inversions, each recessionary episode was matched with the most recent preceding inversion, and the elapsed time between inversion onset and the official NBER recession start date was measured. The results indicate that inversions preceded recessions by an average of approximately 11 months, with individual lead times ranging from 5 months prior to the 1990 recession to 17 months prior to the 1980 recession.
The consistency of this signal across multiple business cycles each shaped by distinct structural, monetary, and exogenous conditions reinforces its robustness as a forward-looking indicator. From an institutional perspective, an average lead time of 11 months provides meaningful scope for preemptive action: financial institutions can use inversion signals to reassess funding strategies, adjust interest-rate hedging positions, review liquidity buffers, and stress-test balance-sheet exposures well in advance of an economic downturn.

# Conclusion
This study provides robust empirical evidence that the 10Y–2Y U.S. Treasury yield spread is an effective leading indicator of economic recessions. Across 600 monthly observations spanning five decades, the yield curve demonstrated a consistent and economically meaningful relationship with future economic conditions.
Yield curve inversions occurred prior to all major recessionary episodes in the sample. Statistical analysis confirmed a significant negative relationship between the yield spread and recession probability (logistic regression coefficient: −1.429). The comparison of pre-recession and non-recession periods revealed a spread differential of approximately one percentage point, while lead-time analysis established that inversions provided an average of 11 months of advance warning a meaningful horizon for institutional risk management.The results demonstrate that the yield curve is not merely a reflection of prevailing market conditions, but a forward-looking instrument encoding market expectations about future growth, monetary policy, and economic risk.

# source
Federal Reserve Economic Data (FRED)
NBER recession dating


Author-
Pratiksha Tayade
