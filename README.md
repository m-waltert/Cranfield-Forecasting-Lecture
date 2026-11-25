# Cranfield Airport Demand Forecasting Lecture

Teaching materials for Dr Manuel Waltert’s guest lecture on airport demand forecasting under uncertainty at Cranfield University.

## Forecasting laboratory

Download [ForecastingDashboard.html](forecasting-lab/ForecastingDashboard.html?raw=true) and open the downloaded file in a browser. If GitHub displays the HTML source, use **Download raw file**. The dashboard works offline and requires no installation.

The laboratory includes:

- Linear and exponential trend extrapolation, with direct and anchored forecasts.
- Holt’s method with adjustable level and trend smoothing weights.
- Log-demand regression with adjustable intercept, time, COVID and log-GDP coefficients, and two GDP scenarios.
- Residual-based Monte Carlo simulation around the lecture’s forecast baselines.
- The lecture notebook’s annual multiplicative approximation to geometric Brownian motion.

Sliders update the calculations and charts. **Restore fitted values** returns to the estimated parameters. Students can change the forecast origin to compare forecasts with later observations and download data and forecasts as CSV files.

### Data and assumptions

Demand covers 1986–2025 and is expressed in million passengers per annum (MPPA). GDP-per-capita values are synthetic teaching data, available through 2024. GDP for 2025 and later is a scenario assumption.

Simulations use 5,000 paths and pointwise 5th–95th percentile bands. The laboratory documents the model equations, fitting conventions and limitations. The multiplicative simulation follows the lecture’s annual Euler approximation, including clipping negative updates to zero; it is not the exact exponential GBM transition.

## Student exercise

Download [forecasting_exercise.xlsx](exercise/forecasting_exercise.xlsx?raw=true) and complete the tasks in its **MC Simulation** and **GBM** sheets after the lecture.

Solutions are intentionally omitted until the exercise has finished.

## Repository contents

| Path | Purpose |
| --- | --- |
| `forecasting-lab/ForecastingDashboard.html` | Complete offline dashboard |
| `exercise/forecasting_exercise.xlsx` | Student exercise workbook |

The HTML file contains all of its data, styling and calculation code. Students do not need the laboratory’s source files, tests, Python scripts, ZIP archive or a local web server.
