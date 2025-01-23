# Automated Compact Letter Display (CLD) Generator for ANOVA Results

This repository contains a Python script that automates the process of generating **Compact Letter Displays (CLDs)** after performing **Analysis of Variance (ANOVA)**. The script not only performs statistical tests to detect significant differences between groups but also generates clear and interpretable results. By assigning the CLDs directly to the results table, it simplifies the interpretation of complex statistical outcomes. Furthermore, the tool creates visually appealing and publication-ready plots that integrate these displays, making it easy to interpret significant differences between groups at a glance. 

The tool is designed to handle datasets with similar formats efficiently, ensuring both accuracy and scalability. It is particularly useful for researchers and data analysts dealing with repetitive tasks involving ANOVA across multiple datasets. By automating the generation of results and visualizations, this script saves time, minimizes human error, and provides a streamlined workflow for data analysis and presentation.

## Features

- **Automated ANOVA Analysis**: Performs ANOVA to detect significant differences between groups.
- **CLD Generation**: Automatically calculates and generates Compact Letter Displays.
- **Results Table Integration**: Assigns the generated CLDs to the ANOVA results table for clear interpretation.
- **Visualization**: Creates publication-ready plots with CLDs displayed directly on the graph.
- **Reusable and Scalable**: Designed to handle new datasets with similar formats, enabling seamless automation for repetitive tasks.



## Input Data Format

The script expects the input data to have the following structure:

|     | Group              |   Variable 1 |   Variable 2 |   Variable 3 |  Variable 4 |   Variable 5 | 
|----:|:------------------------|---------------:|--------------:|--------------------:|------------------:|------------------------:|
| 139 | Alpha                |        44.275  |         0.65  |              97.048 |            13.608 |                    25   |      
|  49 | Bravo |        29.9    |        -1.925 |              42.446 |             9.814 |                    22.3 |   
| 142 | Danger               |        41.7    |        -1.775 |              63.246 |            12.883 |                    21.2 |             
|  90 | Rodger               |        14.8375 |        10.775 |              40.538 |            16.588 |                    18.5 |                  


- **Group**: Categorical variable representing the treatment or group.
- **Value**: Numerical variable representing the measured outcome.

## Output

- **Results Table**: A CSV file containing the ANOVA results and the corresponding CLDs.
- **Plots**: Visualizations with CLDs displayed directly on the graph for easy interpretation.

## Example

### Input Data:

|     | Group              |   Variable 1 |   Variable 2 |   Variable 3 |  Variable 4 |   Variable 5 | 
|----:|:------------------------|---------------:|--------------:|--------------------:|------------------:|------------------------:|
| 139 | Alpha                |        44.275  |         0.65  |              97.048 |            13.608 |                    25   |      
|  49 | Bravo |        29.9    |        -1.925 |              42.446 |             9.814 |                    22.3 |   
| 142 | Danger               |        41.7    |        -1.775 |              63.246 |            12.883 |                    21.2 |             
|  90 | Rodger               |        14.8375 |        10.775 |              40.538 |            16.588 |                    18.5 |                  

### Output Results Table:

### Example Dataset:

| Treatment              | Variable 1         | Variable 2        | Variable 3    | Variable 4     | Variable 5 |
|------------------------|----------------------|--------------------|----------------------|---------------------|------------------------|
| Alpha             | 33.96 ± 1.54 bc      | 3.06 ± 0.91 a      | 53.16 ± 1.57 c       | 8.40 ± 0.75 c       | 20.27 ± 0.72 b         |
| Bravo | 30.48 ± 0.93 ac      | 4.14 ± 1.23 a      | 51.81 ± 1.70 c       | 4.49 ± 1.16 b       | 21.44 ± 0.83 b         |
| Danger              | 28.81 ± 0.50 a       | 4.66 ± 1.38 a      | 65.70 ± 3.63 a       | 16.62 ± 0.59 a      | 19.48 ± 1.19 b         |
| Rodger    | 36.70 ± 0.93 b       | 5.92 ± 0.63 a      | 43.16 ± 0.86 b       | 6.57 ± 0.71 bc      | 28.93 ± 1.03 a         |
| p-value              | 0.0001***            | 0.2932ns           | 0.0000***            | 0.0000***           | 0.0000***              |

- **Interpretation**:
  - Values with different letters (e.g., `a`, `b`, `c`) in the same column indicate statistically significant differences.
  - p-values indicate the level of significance: `***` for highly significant, `ns` for not significant.

### Example Visualization

Below is an example of the generated visualization with Compact Letter Displays:

![CLD Plot Example](Visualization(Figures)/cld_plot.png)


## Contributing

Contributions are welcome! If you have ideas for improvement or encounter any issues, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or suggestions, feel free to reach out:

- Email: [Jabulente@hotmail.com](Jabulente@hotmail.com)
