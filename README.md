# Project 1 (Tactile-Ultrasound (US) signal fusion) dataset

These are the different training and testing datasets organized to generate the tactile-US signal sets.

### 1. 
- Each of all the folders in this repository has two sub-folders labeled as "tumor" and "nontumor". These are also labels to the tactile-US data stored in them.

### 2. 
- A tactile-US image visualized in 3D.

![Tctile-US image in 3D](Resources/In_3D.bmp)

### 3. 
- At the time of acquisition, the tactile and the US images are aligned and visualized in 2D as following.

<font color="red">____________.</font>![Tctile-US image in 2D](Resources/sample_tactile-US_img.png)

4. Notice that in the 3D image where the tactile image plane intersects the US image plane, the US image area above the line of intersection is irrelevant and is 
therefore blancked out.
5. Each of the 2D images is converted to intensity signals in row-wise manner and saved as numerical 2D matrix in a .txt file.
6. The folders "train" and "test" in this repository contains the original tactile and US paired images organized into tumor and nontumor categories.
7. Folders "train_signal_series_with_original_shape" and "test_signal_series_with_original_shape" contain the paired tactile-US signal series that reflect the entire 
dimensions of each of the images, respectively.
8. Folders "train_us_signal_org_shape" and "test_us_signal_org_shape" contain only the US signal series extracted from the folders in 7.
9. Folders "train_signal_series_0" and "test_signal_series_0" contain the same as that in 7; however, the US signals only reflect the relevant area of the US image 
that is below the line of intersection.
10. Folders "train_signal_series_t" and "test_signal_series_t" contains only the tactile signal series extracted from the folders in 9.
11. Folders "train_signal_series_u" and "test_signal_series_u" contains only the US signal series extracted from the folders in 9.
