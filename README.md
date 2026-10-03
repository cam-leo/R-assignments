# R Projects

R work from university courses, plus an Exam PA-style analysis.

## Exam PA: Health Insurance Analysis

`PA_healthinsurance.Rmd` ([rendered report](PA_healthinsurance.html)) explores what drives health insurance charges and builds a regression model to predict them. The data is in `data/health_insurance.csv`, so the report runs as is:

```r
rmarkdown::render("PA_healthinsurance.Rmd")
```

Main findings: smoking is by far the biggest factor, and its effect is much larger for people with a BMI of 30 or more. A model that includes this smoker × obesity interaction explains about 87% of the variation in charges, compared with 75% without it.

## Course Assignments

| File | Course |
|---|---|
| `STAC51_A1.Rmd`, `STAC51 A2.Rmd`, `STAC51A3.Rmd` | STAC51: Categorical Data Analysis |
| `stad37 a1.Rmd`, `STAD37 A2.Rmd`, `stad37 a3.Rmd` | STAD37: Multivariate Analysis |
| `a1 stac67.Rmd` | STAC67: Regression Analysis |
| `stac58 a1.Rmd` | STAC58: Statistical Inference |
| `A1 STAD51.Rmd` | STAD51 |

Some assignments read course data files that aren't in this repository (`pollution.csv`, `p1_4.txt`, `data_chisqplot.txt`, `profilePotato.txt`, `2sample_data.txt`, `t6_17.txt`), so they need those files in the same folder to run. `A1 STAD51.Rmd` downloads market data (quantmod) and Statistics Canada data (cansim), so it needs an internet connection.
