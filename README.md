# Automated Compact Letter Display (CLD) Generator

This repository contains a Python script that automates the process of generating **Compact Letter Displays (CLDs)** after performing **Analysis of Variance (ANOVA)**. The script assigns the CLDs to the results table and creates plots that integrate these displays, making it easy to interpret significant differences between groups. The tool is designed to handle datasets with similar formats efficiently, saving time and ensuring accuracy.

## Features

- **Automated ANOVA Analysis**: Performs ANOVA to detect significant differences between groups.
- **CLD Generation**: Automatically calculates and generates Compact Letter Displays.
- **Results Table Integration**: Assigns the generated CLDs to the ANOVA results table for clear interpretation.
- **Visualization**: Creates publication-ready plots with CLDs displayed directly on the graph.
- **Reusable and Scalable**: Designed to handle new datasets with similar formats, enabling seamless automation for repetitive tasks.



## Input Data Format

The script expects the input data to have the following structure:

| Group  | Value  |
|--------|--------|
| A      | 12.5   |
| A      | 13.0   |
| B      | 15.2   |
| C      | 10.8   |

- **Group**: Categorical variable representing the treatment or group.
- **Value**: Numerical variable representing the measured outcome.

## Output

- **Results Table**: A CSV file containing the ANOVA results and the corresponding CLDs.
- **Plots**: Visualizations with CLDs displayed directly on the graph for easy interpretation.

## Example

### Input Data:

| Group  | Value  |
|--------|--------|
| A      | 12.5   |
| A      | 13.0   |
| B      | 15.2   |
| C      | 10.8   |

### Output Results Table:

### Example Dataset:

| Treatment              | Plant height         | Leaf number        | Fresh biomass (g)    | Dry biomass (g)     | Days to 1st flowering | Number of pods per plant | Number of seeds per pod | Weight of 100 seeds (g) | Yield (g)            |
|------------------------|----------------------|--------------------|----------------------|---------------------|------------------------|--------------------------|--------------------------|--------------------------|----------------------|
| Herbicide             | 33.96 ± 1.54 bc      | 3.06 ± 0.91 a      | 53.16 ± 1.57 c       | 8.40 ± 0.75 c       | 20.27 ± 0.72 b         | 13.11 ± 0.85 c          | 5.09 ± 0.74 a           | 37.65 ± 0.75 a          | 1621.84 ± 25.65 c    |
| Hoeing and Weed Removal| 30.48 ± 0.93 ac      | 4.14 ± 1.23 a      | 51.81 ± 1.70 c       | 4.49 ± 1.16 b       | 21.44 ± 0.83 b         | 18.77 ± 0.49 b          | 6.17 ± 0.56 a           | 37.02 ± 0.93 a          | 1602.16 ± 62.48 c    |
| Mulching              | 28.81 ± 0.50 a       | 4.66 ± 1.38 a      | 65.70 ± 3.63 a       | 16.62 ± 0.59 a      | 19.48 ± 1.19 b         | 22.42 ± 0.47 a          | 6.62 ± 0.68 a           | 35.18 ± 0.62 a          | 2394.25 ± 10.71 a    |
| No Weed Management    | 36.70 ± 0.93 b       | 5.92 ± 0.63 a      | 43.16 ± 0.86 b       | 6.57 ± 0.71 bc      | 28.93 ± 1.03 a         | 7.80 ± 1.07 d           | 4.25 ± 0.95 a           | 35.16 ± 0.79 a          | 959.95 ± 39.04 b     |
| p-value              | 0.0001***            | 0.2932ns           | 0.0000***            | 0.0000***           | 0.0000***              | 0.0000***               | 0.1453ns                | 0.0669ns                | 0.0000***            |

- **Interpretation**:
  - Values with different letters (e.g., `a`, `b`, `c`) in the same column indicate statistically significant differences.
  - p-values indicate the level of significance: `***` for highly significant, `ns` for not significant.

### Visualization:
A bar plot or box plot with Compact Letter Displays shown above each group.


## Contributing

Contributions are welcome! If you have ideas for improvement or encounter any issues, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or suggestions, feel free to reach out:

- LinkedIn: [Your LinkedIn Profile](#)
- Email: [Your Email Address](#)
