# Computer-Vision Tasks


# CV-A01: Images, Filters, Histograms, Gradients, Frequency

## Objectives
- Filtration of noisy images using low pass filters such as: average, Gaussian, median.
- Edge detection using variety of masks such as: Sobel, Prewitt, and canny edge detectors.
- Histograms and equalization.
- Frequency domain filters.
- Hybrid images.

## Deadline
**Wednesday 8 Mar 2023 at 11:59 PM**

## Deliverables
- Filters.py : this will include you implementation for filtration functions (requirements 1-3)
- Frequency.py : this will include your implementation for histogram related tasks (requirements 4-8).
- Histograms.py : this will include your implementation for frequency domain related tasks (requirements 9-10).
- Images : folder contains images to test your implementation.
- UI necessary files

## GUI
Create three tabs:
- Tab 1 : load and show input image, choose a filter from list of available filters, determine filter parameters, apply the fiter then show the output image.
- Tab 2 : load and show input image, calculate and plot input image histogram, apply histogram equalization and show output image, plot output histogram.
- Tab 3 : load input image A, load input image B, make and show hybrid image.


# CV-A02
## Objectives
* Apply Hough transform for detecting parametric shapes like circles and lines
* Apply Active Contour Model for semi-supervised shape delineation.


## Three python files 
* **Hough.py**: includes implementation for Hough transform for lines, circles, and Ellipses.
* **ActiveContour.py**: includes implementation for Active Contour Model for semi-supervised shape delineation and the ChainCode  of the Contour.
* **App.py**: The main file for GUI using Streamlit open-source framework.


# Implemented Functions

## Hough-Line-Detection
Implementation of Simple Hough Line Detection Algorithm in Python.

### Input
The script requires one positional argument and few optional parameters:
* image_path : Complete path to the image file for circle detection.
* bin_threshold : Thresholding value . Default is 150.
* min_edge_threshold : Minimum threshold value for edge detection. Default 100.
* max_edge_threshold : Maximum threshold value for edge detection. Default 200.

### Output

![line](https://user-images.githubusercontent.com/93046966/227671967-7a7530a4-7c08-4c2a-b3b5-9a65fb58be85.png)



## Hough-Circle-Detection
Implementation of Simple Hough Circle Detection Algorithm in Python.

### Input
The script requires one positional argument and few optional parameters:
* image_path : Complete path to the image file for circle detection.
* bin_threshold : Thresholding value . Default is 150.
* min_edge_threshold : Minimum threshold value for edge detection. Default 100.
* max_edge_threshold : Maximum threshold value for edge detection. Default 200.

### Output

![circle](https://user-images.githubusercontent.com/93046966/227671683-02171c70-83f1-4540-9ed4-20fdca20a016.png)



## Hough-Ellipse-Detection
Implementation of Simple Hough Circle Detection Algorithm in Python.

### Input
The script requires one positional argument and few optional parameters:
* image_path : Complete path to the image file for circle detection.
* bin_threshold : Thresholding value . Default is 150.
* min_edge_threshold : Minimum threshold value for edge detection. Default 100.
* max_edge_threshold : Maximum threshold value for edge detection. Default 200.

### Output
![Ellipse](https://user-images.githubusercontent.com/93046966/227672233-60740bf8-5bbe-42ec-8d34-ef422c826c3b.png)



## Active-Contour
Implementation of Simple Active Contour Snake Algorithm in Python.

### Input
The script requires two positional arguments and few optional parameters:
* image : ND array of input image in gray-scale after applying guassian filter.
* snake : ND array of points of the inital snake.
* alpha : weight of elasticity component of snake. Default 0.01.
* beta : weight of stiffness component of snake. Default 0.1.
* w_line : weight of attraction force to brightness of input image. Default 0.0.
* w_edge : weight of attraction to edges of input image. Default 1.0.
* gamma : weight of energy that forces the snake toward or away from edges. Default = 0.01.
* max_px_move : Maximum pixel distance to move per iteration. Default = 1.0.
* max_num_iter : Maximum iterations to optimize snake shape. Default = 2500.

### Output
![active_contour](https://user-images.githubusercontent.com/81927516/227679157-dd6f64f0-e5ac-4e7f-92a2-5b25af92f97c.png)



## Chain Code
Implementation of Simple Chain Code calculation for Snake Algorithm in Python.

### Input
The script requires one positional argument:
* snake : array of the final snake calculated.

### Output
![chaincode](https://user-images.githubusercontent.com/81927516/227679958-ef3e8d80-41ab-4f5d-ab71-83dbbdeb153c.png)

# CV-A03
## Objectives
* Harries Algorithm
* SIFT Algorithm
* Feature Matching

## Harries Algorithm

The Harris corner detection function is used for identifying corners and inferring features of an image. Corners are the important features in the image, which are invariant to translation, rotation, and illumination.

* Original Image

![Original Image](https://user-images.githubusercontent.com/37380802/231598285-bb96a0c2-f536-4da7-91c2-421d56b88e98.PNG)

* After Applying Harris Algorithm

![After Applying Harris Algorithm](https://user-images.githubusercontent.com/37380802/231598595-dfa3d487-1fd0-4160-bc69-5861a0cca1d1.PNG)

* UI Apperrance

![image](https://user-images.githubusercontent.com/37380802/231603173-5127760a-f5bd-4d42-8d33-beb24115c5fa.png)


## SIFT Algorithm

SIFT Scale-Invariant Feature Transform (SIFT) is another technique helps locate the local features in an image, commonly known as the ‘keypoints‘ of the image. These keypoints are scale & rotation invariants that can be used for various computer vision applications.

* Original Image

![image](https://user-images.githubusercontent.com/37380802/231601912-f4e8c6bb-c26d-4061-b57d-6cb41e981451.png)

* After Applying SIFT

![image](https://user-images.githubusercontent.com/37380802/231602024-a35541a7-871e-4b3b-a0f9-86842f9c1dff.png)

## Feature Matching
* Using SSD
  
![SSD](https://user-images.githubusercontent.com/37380802/231600979-1da9e9ef-0883-48c7-a1b8-2ad7f90725b7.jpeg)
  
* Using Normalized Correlation (NCC)
 
![NCC](https://user-images.githubusercontent.com/37380802/231601282-cb53cc4c-99d2-481d-8b97-f6cd380890cd.jpeg)

* UI Apperrance

![image](https://user-images.githubusercontent.com/37380802/231603915-32b6880a-9352-4430-95e9-9c45bf4b8699.png)

## About Us

### Team  Number 8 

### Members

Name| Section | Bench Number |
--- | --- | --- |
[Maryam Megahed](https://github.com/MaryamMegahed "Maryam Megahed") | 2 | 34
[Arwa Essam](https://github.com/arwa-essam "Arwa Essam") | 1 | 12
[Shrouk Shawky](https://github.com/shirouq-shawky "Shrouk Shawky") | 1 | 46
[Sohaila Mahmoud](https://github.com/sohailamahmoud "Sohaila Mahmoud") | 1 | 45
