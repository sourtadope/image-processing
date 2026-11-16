# Image Processing

Classical computer vision in Python: from histogram equalisation and filtering to segmentation and object counting. Jupyter notebooks, OpenCV, NumPy, SciPy, Matplotlib.

## Highlights

**[Flood-area segmentation](flood_segmentation_notebook-2.ipynb)** — segments flooded areas in photos from the Kaggle dataset `faizalkarim/flood-area-segmentation`. Instead of one fixed threshold for every image, it uses the dataset's metadata to choose the thresholding per image, then cleans the mask with morphology and connected components. Predictions are scored against ground-truth masks, compared by image category and against an Otsu baseline.

**[Rice grain counter](Lab_12_2(Rice_counter).ipynb)** — counts touching grains in a photo: CLAHE contrast, Otsu threshold, morphological opening, distance transform and watershed to split grains that touch, then contours to count them.

## All notebooks

| Notebook | Topic |
|---|---|
| [Lab 5](Lab%205/lab5.ipynb) | Histogram equalisation, colour channels |
| [Lab 6-2](Lab%206-2/lab6.ipynb) | Smoothing filters (box, Gaussian), custom kernels, Sobel |
| [Lab 7-1](Lab%207-1/lab7-1.ipynb), [Lab 7-2](Lab%207-2/Lab%207-2.ipynb) | Edge detection: Sobel, Laplacian, Canny |
| [Lab 9-1](Lab%209-1/lab%209-1.ipynb) | Image restoration and denoising: noise models, mean and order-statistic filters ([report](Lab%209-1/lab9_report.txt)) |
| [Lab 10-2](Lab_10_2.ipynb) | Gradients and thresholding |
| [Lab 12-2](Lab%2012-2.ipynb) | Morphology and labelling on a synthetic image |
| [Lab 13](Lab13.ipynb) | Classical segmentation: Otsu and adaptive thresholds, morphology, connected components |
| [Colour image processing](Color_Image_Processing_Student_Workbook%20(1).ipynb) | Colour models, pseudocolour, colour slicing, colour histograms, smoothing and sharpening |

## Run
Open any notebook in Jupyter or Google Colab. Requirements: `opencv-python`, `numpy`, `scipy`, `matplotlib` (the flood notebook also uses `kagglehub` and `pandas`).
