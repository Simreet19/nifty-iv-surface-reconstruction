# NIFTY IV Surface Reconstruction

## Overview

This project focuses on reconstructing missing implied volatility (IV) values in NIFTY option data while preserving the natural structure of the volatility surface.

## Problem

The dataset contains missing IV values across option strikes. The objective is to accurately estimate these missing values while maintaining:

* Volatility smile
* Volatility skew
* Surface smoothness
* Financial consistency

## Methodology

The final approach uses:

1. Log-Moneyness Transformation
2. Row-wise Akima Interpolation
3. CE/PE Specific Extrapolation
4. Column-wise Akima Fallback
5. Linear Fallback for Remaining Missing Values

## Results

Final validation MSE: 0.0000425568

## Technologies

* Python
* Pandas
* NumPy
* SciPy
* Matplotlib

## Future Improvements

* Surface fitting methods
* XGBoost-based reconstruction
* Time-series aware models
* Arbitrage-free IV surface constraints

