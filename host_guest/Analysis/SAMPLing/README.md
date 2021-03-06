# Analysis of the SAMPLing challenge

Preliminary analysis of the SAMPLing challenge.

Another set of reference calculations has been performed, and we are currently trying to resolve differences in the
final free energies on the order of 1-1.5 kcal/mol. We'll update the analysis once we understand the cause of the
discrepancies.

## Manifest

- `Plots/`: Plots of the free energy predictions in times with 95% t-based confidence intervals computed using the data
  of the 5 replicates.
- `Data/`: CSV and JSON data for the reference calculations and submission analysis.
  - `submission_id.csv/json`: contain the mean free energy, the 95% t-based confidence interval, and the difference
     with the reference calculation in time for all three systems. The values of the confidence interval (`DG_CI`) have
     to be interpreted as `mean-DG +- DG_CI`
  - `reference_free_energies.csv/json`: contain the free energies of all 5 replicates, number of energy evaluations,
     CPU time, mean free energy, and 95% t-based confidence interval in time for all the three systems.
