# Catastrophe Risk Modeling & Portfolio Loss Simulation

## Overview
This project models financial risk from natural disasters (floods and storms) on an insurance portfolio using historical data and Monte Carlo simulation.

## Objective
Estimate:
- Expected Annual Loss (EAL)
- Tail risk (95% Value at Risk)

## Data
- Disaster data: EM-DAT (historical catastrophe events)
- Portfolio data: Synthetic insurance exposure dataset (assets, risk zones, insured values)

## Methodology
1. **Data Filtering**
   - Country: India
   - Disaster types: Flood, Storm

2. **Frequency Modeling**
   - Poisson distribution  
   - Avg events/year (λ): **3.96**

3. **Severity Modeling**
   - Lognormal distribution  
   - μ = **18.93**, σ = **2.22**

4. **Monte Carlo Simulation**
   - Simulated annual catastrophe events
   - Estimated portfolio losses across 500+ scenarios

## Results
- **Expected Annual Loss (EAL):** $177M  
- **95% Value at Risk (VaR):** $343M  

## Key Insights
- Moderate event frequency but high financial impact  
- Loss distribution is heavy-tailed (extreme events dominate risk)  
- Portfolio exposed to significant tail risk  

## Tech Stack
- Python (Pandas, NumPy, SciPy)
- Matplotlib
- Monte Carlo Simulation

## Conclusion
The model shows that while average losses are manageable, extreme events can lead to substantial financial impact, highlighting the importance of reinsurance and risk diversification.
