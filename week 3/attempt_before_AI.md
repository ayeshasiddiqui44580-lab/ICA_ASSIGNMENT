# Referee's Note & Metric Selection (Before AI)

## 1. Metric Selection Strategy
- **Skewed Items (with Flagged Outliers):** I will report the **Median** because extreme flagged values pull the mean upward, making the average look artificially high while the median is a more representative measure.
- **Stable Items (without Outliers):** I will report the **Mean** because prices are symmetrically distributed without extreme spikes.
- **Trend Over Time:** I will report the **First-to-Last Percentage Change** alongside the median to show overall price movement from the start to the end of the period.

# 2. Referee's Note (Labelled with O, E, C)
[O] The median price for staple items did not change much over time if we looked at the ledger period, whereas the mean price was pulled up by some extreme price entries.  [O] Removing the flagged outlier rows from the dataset causes the mean to drop significantly and become much closer to the median.[O] Retail prices show an overall upward drift from earliest to latest date for which data are available, as measured by a calculation of first-to-last percentage change. [E]One explanation for the gap between the mean and median could be isolated supply chain disruptions or bulk-entry errors that were recorded on certain dates. [C] These isolated price spikes caused the arithmetic mean to overstate the average daily cost faced by consumers. [O] Hence, quoting the median gives a better picture of the average price than the mean.