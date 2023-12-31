# MIT_BIH_ECGs
### Submit research results to IEEE ICCE-TW 2023 
## The goal of our paper
Our novel approach transforms the segmented time-series into two-dimensional images, improving feature coverage and highlighting differences between arrhythmia types.

This study used the MIT-BIH arrhythmia database for research design and experiments. The following is a detailed description of each step:

### Step 1: 
In this study, the ECG time-series signal in the MIT-BIH dataset is divided into t1 before point R and t2 after point R, where t1 has 90 nodes and t2 has 166 nodes. The segmented ECG signal was filtered and denoised using AEs. AEs can improve the quality of the signal and reduce noise. 

![image](https://github.com/tsubasa-k/MIT_BIH_ECGs/assets/61736148/281ebeec-c644-4469-9a2d-230f8c370ff5)

Comparison results of 1D ECG signal before and after noise reduction

### Step 2: 
In contrast to previous studies, we not only used segmented 1D time-series to train classification models, but also visualized the segments as 2D images. 
This approach maximizes feature coverage, accentuates differences between image feature categories, and enhances the training results of the classification model.

This study uses the Gramian angular field to convert a 1D time series into 2D images, which are divided into two methods: summation and difference

![image](https://github.com/tsubasa-k/MIT_BIH_ECGs/assets/61736148/a9b28b83-6196-436f-a38b-0be4afd2d4b0)

Two-dimensional image
 (Left: Summation; Right: Difference)

### Step 3: 
The results of 1D ECG signal denoising and 2D image datasets were divided into training and test sets for CNN training and prediction.

### Step 4: 
The developed model utilized the D1 mini single-chip development version and the AD8232 ECG sensor to measure heart rate.

![image](https://github.com/tsubasa-k/MIT_BIH_ECGs/assets/61736148/90c56fa1-9587-439b-9807-1c103c89a145)

AD8232(left) and D1 mini(right)










