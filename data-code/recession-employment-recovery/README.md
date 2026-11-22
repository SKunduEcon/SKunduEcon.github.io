# Data and code: US employment recovery

This folder contains a reproducible Jupyter notebook for the historical US payroll-employment recovery chart used in [How AI Changes the Recession Recovery Math](https://skunduecon.github.io/research/ai-changes-the-recovery-math.html).

## Contents

- `recovery_months.ipynb`: recreates a bar chart of the number of months required for US payroll employment to regain its pre-recession level across four recession episodes.

## Data and source

The notebook uses the four episode-level values reported in RAND's July 2022 commentary:

| Recession episode | Months to regain pre-recession payroll employment |
|---|---:|
| 1990–91 | 31 |
| 2001 | 46 |
| 2007–09 | 77 |
| 2020 | 29 |

Source: [RAND, Recovered but not whole: US jobs rebounded after the pandemic, but employment recovery differs across recessions](https://www.rand.org/pubs/commentary/2022/07/recovered-but-not-whole-us-jobs-rebounded.html).

## Reproduce

Open the notebook in Jupyter or Google Colab and run all cells. It requires Python 3 and Matplotlib.

## Interpretation

These are descriptive comparisons of distinct recession episodes. The 2020 contraction was a pandemic shutdown shock followed by rapid reopening, so its recovery time is not directly comparable with earlier episodes involving slower cyclical and structural adjustment. The chart does not identify the causal effect of AI or technology on employment recovery.
