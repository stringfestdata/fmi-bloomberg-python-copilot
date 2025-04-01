**Monte Carlo Simulation for IRR Calculation**

**Objective:**
Calculate the Internal Rate of Return (IRR) for a project over three years, incorporating uncertainty in cash flows through Monte Carlo simulation.

**Inputs and Distributions:**
1. **Initial Investment**:
   - Description: Fixed cash outflow at the start of the project (Year 0).
   - Value: -$100,000

2. **Cash Flow Period 1 (Year 1)**:
   - Description: Expected cash flow with uncertainty.
   - Distribution: Uniform
   - Parameters: Min = $20,000, Max = $40,000

3. **Cash Flow Period 2 (Year 2)**:
   - Description: Expected cash flow with uncertainty.
   - Distribution: Normal
   - Parameters: Mean = $50,000, Standard Deviation = $5,000

4. **Cash Flow Period 3 (Year 3)**:
   - Description: Expected cash flow with uncertainty.
   - Distribution: Triangular
   - Parameters: Min = $40,000, Most Likely = $60,000, Max = $80,000

**Simulation Settings:**
- **Number of Periods**: 3 years
- **Number of Simulations**: 10,000 iterations
- **Correlation**: Include a slight positive correlation (0.3) between revenue and costs if applicable.

**Constraints:**
- Ensure all cash flows are non-negative (Cash flows ≥ $0).

**Output and Visualization:**
- Calculate the IRR for each simulation run and derive statistics (mean, median, confidence intervals) about the IRR from the simulation results.
- **Visualizations:**
  - **Histogram**: Display a histogram of the IRR results to visualize the distribution and identify the spread and skewness of IRR outcomes.
  - **Box Plot**: Use a box plot to highlight the median, quartiles, and any outliers in the IRR data.
  - **Probability Density Plot**: A smoothed probability density plot to see the density of different IRR ranges, giving a clear visual of the most probable IRR outcomes.
  - **Cumulative Distribution Function (CDF) Plot**: This plot will show the probability of achieving an IRR less than or equal to each value, helpful for risk assessment.

**Procedure:**
1. Generate cash flows for each year based on specified distributions.
2. Calculate IRR for each set of yearly cash flows across all simulations.
3. Aggregate the IRR results to analyze the distribution and assess the risk and return profile of the investment.
4. Visualize the results using the described plots to provide a comprehensive overview of the potential IRR outcomes.

**Analysis:**
- Review the distribution of the IRR results to understand the likelihood of achieving various IRR thresholds.
- Determine the probability of achieving an IRR above a specific target (e.g., the company's cost of capital).
- Use visualizations to present findings in a clear and accessible manner to stakeholders.
