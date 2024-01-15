# TSSDA-Lab

<a target="_blank" href="https://colab.research.google.com/github/kbdharun/TSSDA-Lab">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a><br><br>

This repository contains the programs that I worked out in Time Series and Sequential Data Analysis Lab.

This repository contains the programs that I worked out in Machine Learning Laboratory.

## Index

- Lab 1: Introduction
  - [Prelab: Exploring Pandas and Matplotlib](prelab/prelab.ipynb)
  - [Task 1: Viewing Time Series Data](lab1/TSA-Ex1-task1.ipynb)

## Prerequisites

Python and packages in `requirements.txt` file installed.

> [!NOTE]
> You can install all the packages in the file using the command `pip install -r requirements.txt`.

### Container Image

Alternatively, you can use the [container image](https://github.com/kbdharun/TSSDA-Lab/pkgs/container/tssda-lab-image) I created with all the packages preinstalled.

You can install it in [Distrobox](https://github.com/89luca89/distrobox) with the command `distrobox create -i ghcr.io/kbdharun/tssda-lab-image:latest -n ml` and use it with the command `distrobox enter ml`.

Additionally, you can verify the authenticity of the container image using [`cosign`](https://github.com/sigstore/cosign) (download the `cosign.pub` file from [here](https://github.com/kbdharun/TSSDA-Lab/blob/main/cosign.pub) and execute the following command):

```zsh
cosign verify --key cosign.pub ghcr.io/kbdharun/tssda-lab-image:latest
```
