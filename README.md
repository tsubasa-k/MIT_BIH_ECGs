# MIT_BIH_ECGs
## Step 1: 
In this study, the ECG time-series signal in the MIT-BIH dataset is divided into t1 before point R and t2 after point R, where t1 has 90 nodes and t2 has 166 nodes. The segmented ECG signal was filtered and denoised using AEs. AEs can improve the quality of the signal and reduce noise. 

![image](https://github.com/tsubasa-k/MIT_BIH_ECGs/assets/61736148/281ebeec-c644-4469-9a2d-230f8c370ff5)

## Step 2: 
Unlike prior studies, we not only used segmented 1D time series for training classification models but also visualized the segments as 2D images. 
This approach maximizes feature coverage, accentuates differences between image feature categories, and enhances the training results of the classification model.

This study uses the Gramian angular field to convert a 1D time series into 2D images, which are divided into two methods: summation and difference

![image](https://github.com/tsubasa-k/MIT_BIH_ECGs/assets/61736148/a9b28b83-6196-436f-a38b-0be4afd2d4b0)



