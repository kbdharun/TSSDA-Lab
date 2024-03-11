# TSSDA-Lab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kbdharun/TSSDA-Lab)
[![CodeFactor](https://www.codefactor.io/repository/github/kbdharun/tssda-lab/badge)](https://www.codefactor.io/repository/github/kbdharun/tssda-lab)

This repository contains the programs that I worked out in Time Series and Sequential Data Analysis Lab.

## Index

- Lab 1: Introduction
  - [Prelab: Exploring Pandas and Matplotlib](prelab/prelab.ipynb)
  - [Task 1: Viewing Time Series Data](lab1/TSA-Ex1-task1.ipynb)
- Lab 2: Basic Feature Engineering with Time Series Data
  - [Task 2: Feature Engineering Program](lab2/TSSDA-Ex2.ipynb)
- Lab 3: ITSM Tool Exploration
- Lab 4: Data Visualization and Sampling
  - [Task 3: Data Visualization Program](lab4/Ex3-Visualization.ipynb)
  - [Task 4: Data Sampling Program](lab4/Ex4-Sampling.ipynb)
- Lab 5: Check the Stationality, Trend and Seasonality
  - [Task 5A](lab5/TS-Exp5A.ipynb)
  - [Task 5B](lab5/TS-Exp5B.ipynb)
- Lab 6: Check the Stationality, Trend and Seasonality
  - [Task 5C](lab6/TS-Exp5C.ipynb)
  - [Task 6A: Check for the ACF and PACF of the data](lab6/TS-Exp6A.ipynb)

----

- Lab 7: ACF, PACF, AR, MA, ARMA calculations
  - [Task 6A: Check for the ACF and PACF of the data](lab7/TS-Exp6A.ipynb)
  - [Task 6B: Check for the ACF and PACF of the data](lab7/TS-Exp6B.ipynb)

- Lab 7 (continued): Implement the differencing method and polynomial model to create a seasonally adjusted time series
  - [Task 7](lab7/TS-Exp7.ipynb)
  - [Task 7A](lab7/TS-Exp7A.ipynb)
  - [Task 7A](lab8/TS-Exp7A-Sunspots.ipynb) (using Sunspots dataset)

- Lab 8: ARMA; OLS, GLS, Rolling Regression; Evaluating Performance Metrics
  - [Task 8: ARMA](lab8/TS-Exp8-ARMA.ipynb)
  - [Task 8A: OLS, GLS, Rolling Regression](lab8/TS-Exp8-OLS,GLS,Rolling_Reg.ipynb)
  - [Task 8B: Evaluating Performance Metrics](lab8/TS-Exp8-Metrics.ipynb) (only for reference)

## Prerequisites

Python and packages in `requirements.txt` file installed.

> [!NOTE]
> You can install all the packages in the file using the command `pip install -r requirements.txt`.

### Container Image

Alternatively, you can use the [container image](https://github.com/kbdharun/TSSDA-Lab/pkgs/container/tssda-lab-image) I created with all the packages preinstalled.

You can install it in [Distrobox](https://github.com/89luca89/distrobox) with the command `distrobox create -i ghcr.io/kbdharun/tssda-lab-image:latest -n tssda` and use it with the command `distrobox enter tssda`.

Additionally, you can verify the authenticity of the container image using [`cosign`](https://github.com/sigstore/cosign) (download the `cosign.pub` file from [here](https://github.com/kbdharun/TSSDA-Lab/blob/main/cosign.pub) and execute the following command):

```zsh
cosign verify --key cosign.pub ghcr.io/kbdharun/tssda-lab-image:latest
```
