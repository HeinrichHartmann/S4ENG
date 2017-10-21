# Statistics for Engineers

## TOC

0. Foreword

0. Introduction
   - Information needs in IT Operations/Software Engineering
   - Available Data Sources: Monitoring/Logs/Tracers -> We mainly focus on monitoring data
   - Data Analysis tools, and how to apply them:
     - Data Science: Python/R
     - Ops Tools: Circonus/Graphite, etc.

1. Visualizing Data
   - Abstract data sets:
     - bags of samples
     - bags of tuples
     - time series
   - Available Graphs: Line Plots, Scatter Plots, Rug Plots, Histograms
   - Problems caused by data aggregation: Spike Erosion

2. Visualizing Data in Practice
   - What makes a great Chart? -> Units/Legend/etc.
   - Discussion of charts found in monitoring tools

3. Summary Statistics
   - centrality measures: mean, median, truncated mean
   - dispersion measures: variance, stddev, IQR, mad
   - robustness

3. Summary Statistics in Practice
   - Service Availablility
   - Jitter
   - SLAs

4. Percentiles and Histograms
   - CDF and Counts
   - Percentiles
   - Histogram as data format
   - Mergability of summary statistics

5. Percentiles and Histograms in Practice
   - API Monitoring
   - Percentile charts, Latency band charts, Histogram heatmaps
   - Data aggregation accross nodes

5. Comparing Distributions
   - Parmetric / non-parametric methods: Do we have a good model?
   - Graphical Methods: Histograms, QQ Plots
   - The bootstrap method
   - Hypothesis testing
   - t-test
   - Kolmogorov-Smirnov test

5. Comparing Distributions in Practice
   - A/B tests
   - Detecting performance regressions

6. Regression and Correlation
   - General Curve Fitting problem
   - Linear least squares
   - Correlation Coefficients

7. Regression and Correlation Applications
   - Scalability Analysis: Fitting the USL model to Benchmark data
   - Forecasting with Regressions, Capacity Planning
   - Clustering time series with correlation matrix

8. Time Series Analysis
   - Times Series as iterators
   - Filtering time series basics
   - Exponential Smoothing and Holt Winters
   - CUSUM Change detector
   - A simple Anomaly Detector

9. Time Series Analysis in Practice
   - Alerting!
   - Reducing noise
   - Outlier detection
   - Anomaly detection: When/how to use?

12. Appendix 0: Analytics with Prometheus
    -> Contributed Chapter ??

11. Appendix 1: Analytics with Graphite and IrondDB
    -> Contributed Chapter??

10. Appendix 2: Analytics with Circonus

## Meta Comments

* Audience: We target SysAdmins/SREs/Operations Engineers as primary audience.  However, the content
  of this book applies more generally to people that work with time series data.

* Languages: Math formulas will be supplemented by source code to make them more easy to comprehend
  by the target audience.  We use Python for the examples since it's highly readable and concise,
  and can be translated to other languages easily.

  We don't want this text to be too tool specific.  Applications inside monitoring tools, will be
  discussed in an appendix.

* Content Structure:
  - Chapter's should be short and largely self contained
  - Alternating content: Mathematical Method  then Applications/Examples with real data
  - Q: At the beginning of each chapter we should present some motivation from practice.
    This will be duplicated content.
