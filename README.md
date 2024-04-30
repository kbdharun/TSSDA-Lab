# TSSDA-Lab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kbdharun/TSSDA-Lab)

This repository contains the programs that I worked out in Time Series and Sequential Data Analysis Lab.

## Index

- Lab 1: Introduction
  - [Prelab: Exploring Pandas and Matplotlib](lab00(prelab)/prelab.ipynb)
  - [Task 1: Viewing Time Series Data](lab01/TSA-Ex1-task1.ipynb)
- Lab 2: Basic Feature Engineering with Time Series Data
  - [Task 2: Feature Engineering Program](lab02/TSSDA-Ex2.ipynb)
- Lab 3: ITSM Tool Exploration
- Lab 4: Data Visualization and Sampling
  - [Task 3: Data Visualization Program](lab04/Ex3-Visualization.ipynb)
  - [Task 4: Data Sampling Program](lab04/Ex4-Sampling.ipynb)
- Lab 5: Check the Stationality, Trend and Seasonality
  - [Task 5A](lab05/TS-Exp5A.ipynb)
  - [Task 5B](lab05/TS-Exp5B.ipynb)
- Lab 6: Check the Stationality, Trend and Seasonality
  - [Task 5C](lab06/TS-Exp5C.ipynb)
  - [Task 6A: Check for the ACF and PACF of the data](lab06/TS-Exp6A.ipynb)

----

- Lab 7: ACF, PACF, AR, MA, ARMA calculations
  - [Task 6A: Check for the ACF and PACF of the data](lab07/TS-Exp6A.ipynb)
  - [Task 6B: Check for the ACF and PACF of the data](lab07/TS-Exp6B.ipynb)

- Lab 7 (continued): Implement the differencing method and polynomial model to create a seasonally adjusted time series
  - [Task 7](lab07/TS-Exp7.ipynb)
  - [Task 7A](lab07/TS-Exp7A.ipynb)
  - [Task 7A](lab08/TS-Exp7A-Sunspots.ipynb) (using Sunspots dataset)

- Lab 8: ARMA; OLS, GLS, Rolling Regression; Evaluating Performance Metrics
  - [Task 8: ARMA](lab08/TS-Exp8-ARMA.ipynb)
  - [Task 8A: OLS, GLS, Rolling Regression](lab08/TS-Exp8-OLS,GLS,Rolling_Reg.ipynb)
  - [Task 8B: Evaluating Performance Metrics](lab08/TS-Exp8-Metrics.ipynb) (only for reference)

- Lab 9: ARIMA; Seasonal ARIMA
  - [Task 9: ARIMA](lab09/TS-Exp9,10-ARIMA.ipynb)
  - [Task 10: Seasonal ARIMA](lab09/TS-Exp9,10-ARIMA.ipynb)
  - [Task 11: Multivariate ARIMA forecasting technique](lab09/TS-Exp11A-2.ipynb)

- Lab 10: Implement the state space modelling and visualize the same.
  - [Task 12A: Implement Data GARCH model (without OLS)](lab10/TS-Exp12A.ipynb)
  - [Task 12A: Implement Data GARCH model (with OLS)](lab10/TS-Exp12A-2.ipynb)

- Lab 11: Implement the state space modelling and visualize the same.
  - [Task 12A: Implement Data GARCH model (without OLS)](lab11/TS-Exp12-GARCH.ipynb)
  - [Task 12B: Kalman Filter on Air Quality Dataset](lab11/TS-Exp12-Kalman-Filter.ipynb)
  - [Task 12B: Kalman Filter on Yahoo Finance Dataset](lab11/TS-Exp12-Kalman-Filter-YF.ipynb) (miscellaneous)
  - [Task 12C: Explore and visualize data connected with extreme weather events](lab11/TS-Exp12-Visualization.ipynb) (not required for record)

- [Complete TSSDA Codes Program](TSSDA-Complete-Codes.ipynb)

## Prerequisites

Python and packages in the `requirements.txt` file installed.

> [!NOTE]
> You can install all the required packages using the command `pip install -r requirements.txt`.

### Working with Conda

If you are using `conda` to manage your environments, you can create a new environment for this repository with the command `conda create -n tssda` and activate it with the command `conda activate tssda`.

> [!TIP]
> For faster environment solving in Conda, I would suggesting using the `libmamba` solver. You can set it as the default solver using the command `conda config --set solver libmamba`.

Then, you can install all the required packages using the command `conda install --file requirements.txt`.

### Container Image

Alternatively, you can use the [container image](https://github.com/kbdharun/TSSDA-Lab/pkgs/container/tssda-lab-image) I created with all the packages preinstalled.

You can install it in [Distrobox](https://github.com/89luca89/distrobox) with the command `distrobox create -i ghcr.io/kbdharun/tssda-lab-image:latest -n tssda` and use it with the command `distrobox enter tssda`.

Additionally, you can verify the authenticity of the container image using [`cosign`](https://github.com/sigstore/cosign) (download the `cosign.pub` file from [here](https://github.com/kbdharun/TSSDA-Lab/blob/main/cosign.pub) and execute the following command):

```zsh
cosign verify --key cosign.pub ghcr.io/kbdharun/tssda-lab-image:latest
```
