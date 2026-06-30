HR Attrition Risk Dashboard
Live: https://mrjayvirtual.github.io/HR-Attrition-Risk-Dashboard/
The problem
Most HR dashboards report attrition as a static number. This one ties attrition to a leading indicator — satisfaction score at exit vs. for those who stayed — which is the real analytical question People teams care about: why are people leaving, not just how many.
What it does
An interactive dashboard filtered by department, showing:
Attrition rate with an auto-flagged risk level (stable / elevated / high)
A direct "signal" callout comparing satisfaction scores of leavers vs. stayers
Attrition rate ranked by department (rate, not raw count — a department losing 2 of 3 people is worse than one losing 5 of 50)
Salary band breakdown of who's leaving
Process
Modeled employee-level data: department, tenure, status, satisfaction, salary band
Split the population into cohorts (Left vs. Active) and compared averages — the core technique behind churn analysis in any domain
Ranked departments by attrition rate, correcting for headcount differences
Wrote one explicit insight callout instead of leaving the reader to find the story themselves
Stack
React, inline component state, sample data.
Note
Built with sample/synthetic data for demonstration. The most "transferable analyst" piece of the three — the cohort-comparison logic here maps directly to churn analysis in subscriptions, customers, or any other domain.
