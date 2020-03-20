# Waymo Open Dataset Download Tool

This tool downloads Waymo Open Dataset and converts it into KITTI-like format that consists of individual images and txt labels.

## Prerequisite

* python 2 or 3
* gsutil (command line tool to download files from google cloud)
* waymo_open_dataset (follow the [Quick Start]([https://github.com/waymo-research/waymo-open-dataset/blob/master/docs/quick_start.md]))

## How to use

Before you run the following code, make sure you have set up `gsutil` and `waymo_open_dataset`! Currently only the original training and validation set are supported. Feel free to modify the code to download other data splits.

```
python batch_download.py training --out-dir /ssd/dataset/waymo --resize 1.0
```
