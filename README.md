# Advanced Mathematics for Data Science: Urban Transport Analysis

A computational mathematics project applying calculus, integration, and series approximation to model and analyse urban transport behaviour in Colombo. Built as part of CM2607 – Advanced Mathematics for Data Science at IIT in collaboration with Robert Gordon University.

All work is contained in a single Jupyter Notebook.

## What the notebook covers

**Problem 1: Modelling Travel Time**

Derives and evaluates partial derivatives for bus and taxi travel time functions. Bus travel time follows T_b = ax² + by² and taxi follows T_t = √[c(x² + y²)]. The gradient vectors are computed symbolically using SymPy, then evaluated numerically for a real route (Fort to Borella, 4.5km). A sensitivity analysis compares how each service responds to changes in distance and traffic delay, visualised using 3D surfaces and contour plots with gradient field arrows.

**Problem 2: Cost Analysis Using Integration**

Integrates marginal fare rate functions to compute total fare as a function of distance. Bus fare follows F_b(x) = x² + x and taxi follows F_t(x) = (3/2)x² + 2x. The analysis includes a fare comparison table at multiple distances, consumer surplus estimation, and a percentage premium breakdown showing taxi costs approximately 42% more than bus for a typical urban trip.

**Problem 3: Series Approximation for Peak Travel Times**

Approximates passenger volume using the first four terms of a mixed trigonometric-polynomial series: P(t) = 5 + 4sin(πt) - (3/2)t² + (1/4)t⁴. Two interpretations of the time variable are analysed and compared: direct (t = hours) which becomes physically invalid after roughly 1.7 hours due to polynomial dominance, and normalised (t = hour/24) which remains valid across the full 24-hour cycle. Critical points, rate of change, and truncation error are computed and plotted.

## Libraries used

- SymPy for symbolic differentiation, integration, and series manipulation
- NumPy for numerical evaluation and array operations
- SciPy for FFT utilities and root finding
- Matplotlib for all visualisations including 3D surfaces, contour plots, and time series


## Output figures

The notebook generates the following plots during execution:

- `travel_time_analysis.png` - 3D surfaces and gradient field contour plots for both transport modes
- `sensitivity_analysis.png` - comparative gradient magnitude bar chart
- `fare_analysis.png` - fare comparison, marginal rates, and percentage premium over distance
- `consumer_surplus.png` - economic surplus analysis for bus and taxi services
- `problem3a_direct_interpretation.png` - valid region analysis for direct time interpretation
- `problem3a_interpretation_comparison.png` - side-by-side comparison of both time interpretations
- `problem3a_comprehensive_analysis.png` - full series analysis including rate of change and truncation error

## Author

Sandali Balasooriya - AI & Data Science undergraduate at IIT  
[LinkedIn](https://www.linkedin.com/in/sandalibalasooriya) 