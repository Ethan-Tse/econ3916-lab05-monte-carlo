# econ3916-lab05-monte-carlo
econ3916-lab05-monte-carlo
# Monte Carlo Engine -- Probability & Simulation

## Objective
I used Monte Carlo simulation to estimate probabilities and financial risk, and to check how the error in those estimates shrinks as the number of simulations grows.

## Methodology
- Simulated 10,000 coin flips and plotted the running share of heads to see it settle toward one half.
- Simulated 10,000 Monty Hall games and counted how many times switching doors won.
- Simulated a disease screening test on 100,000 people with 1% prevalence, 95% sensitivity, and 90% specificity, then measured what share of positive tests were actually sick people.
- Computed Monte Carlo Value at Risk (VaR) and Expected Shortfall (ES) for a $1M portfolio over a one-day horizon. VaR is read from a low percentile of the simulated returns, and ES is the average loss on the days at or beyond that VaR.
- Estimated pi at increasing sample sizes and checked that the Monte Carlo error shrinks like 1/sqrt(n).

## Key Findings
- **Monty Hall:** switching won [YOUR VALUE] of 10,000 games.
- **Disease screening:** [YOUR VALUE]% of positive tests were sick people, even though the test is 95% sensitive. The low 1% prevalence means most positives come from the healthy group.
- **Risk:** for the $1M portfolio, 95% VaR is $19,494 and 95% ES is $24,230. ES is larger than VaR because it averages the losses in the tail rather than marking where the tail starts.
- **Convergence:** the pi estimates showed the error shrinking like 1/sqrt(n), so cutting the error in half takes about four times as many simulations.
