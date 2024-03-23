# Audio-Image-CNN

 Audio classification is often proposed as MFCC classification problem. In this project, Audio Classification is performed to map the audios to its 5 major categories. A bonus task of mirroring a video is done. Developed for IT350 assignment 4.

 # Dataset

The ESC-50 dataset is a labeled collection of 2000 environmental audio recordings suitablefor benchmarking methods of environmental sound classification. The dataset consists of 5-second-long recordings organized into 50 semantical classes (with 40 examples per class) loosely arranged into 5 major categories. I will be predicting these audios on these 5 major categories. Clips in this dataset have been manually extracted from public field recordings gathered by the Freesound.org project. 

# Results

## Simple CNN with Parameter Tuning

| Model   | Model Description                                    | Train Loss | Train Accuracy | Validation Loss | Validation Accuracy |
|---------|------------------------------------------------------|------------|----------------|-----------------|---------------------|
| SCNN_1  | Vanilla CNN                                          | 0.9508     | 95.41          | 1.2512          | 66.0                |
| SCNN_2  | With Padding = 1                                     | 0.9512     | 95.41          | 1.2442          | 67.0                |
| SCNN_3  | With Kernel Size 4x4                                 | 0.9816     | 92.47          | 1.2888          | 61.33               |
| SCNN_4  | With Stride 2x2                                      | 1.0612     | 84.94          | 1.2788          | 61.67               |
| SCNN_5  | With More Filters                                    | 0.9530     | 95.12          | 1.2321          | 67.33               |
| SCNN_6  | With Kernel Size 4x4 and Padding = 1                 | 0.9327     | 97.18          | 1.2303          | 67.0                |
| SCNN_7  | With Stride 2x2 and Padding = 1                      | 1.0716     | 84.82          | 1.2527          | 66.33               |
| SCNN_8  | With Kernel Size 4x4, Stride 2x2 and Padding = 1     | 1.0321     | 87.59          | 1.2453          | 66.0                |
| SCNN_9  | With Stride 2x1                                      | 1.0535     | 85.24          | 1.2860          | 61.0                |
| SCNN_10 | With Stride 1x2                                      | 1.0165     | 89.24          | 1.2306          | 67.0                |
| SCNN_11 | With 2 Layers                                        | 0.9554     | 94.88          | 1.2457          | 66.33               |


## Deep CNN with Parameter Tuning

| Model    | Model Description                                       | Train Loss | Train Accuracy | Validation Loss | Validation Accuracy |
|----------|---------------------------------------------------------|------------|----------------|-----------------|---------------------|
| DCNN_1   | Vanilla Deep CNN                                       | 1.2530     | 65.06          | 1.4099          | 49.0                |
| DCNN_2   | With Padding = 1                                      | 1.2777     | 62.35          | 1.3979          | 49.67               |
| DCNN_3   | With Uniform Kernel Size of 3x3                        | 1.2993     | 60.59          | 1.4106          | 49.0                |
| DCNN_4   | With Uniform Kernel Size of 4x4                        | 1.3185     | 58.82          | 1.4890          | 41.33               |
| DCNN_5   | With Uniform Stride of 2x2 and Padding = 2             | 1.3172     | 57.94          | 1.3799          | 52.33               |
| DCNN_6   | With Increased number of Filters                      | 1.6085     | 29.53          | 1.6042          | 30.0                |
| DCNN_7   | With Increased Kernel Size of 5x5 and Padding = 1      | 1.2932     | 61.12          | 1.4604          | 43.67               |
| DCNN_8   | With Uniformly Decreasing Kernel Size                  | 1.1981     | 71.0           | 1.3925          | 50.0                |
| DCNN_9   | With Increased Row Stride                              | 1.3228     | 57.65          | 1.3971          | 49.67               |
| DCNN_10  | With Increased Column Stride                           | 1.2418     | 66.12          | 1.3483          | 55.33               |
| DCNN_11  | With Batch Normalization                               | 1.1320     | 77.65          | 1.2308          | 68.0                |
| DCNN_12  | With Batch Normalisation and Uniformly Decreasing Stride| 1.0842     | 82.82          | 1.2834          | 60.67               |
| DCNN_13  | With Batch Normalisation and Uniform Stride of 2x2 and Padding = 2 | 1.1104 | 79.29          | 1.2120          | 69.0                |
| DCNN_14  | With Batch Normalisation and With Increased Column Stride | 1.1200 | 79.0           | 1.2766          | 62.67               |
| DCNN_15  | With Batch Normalisation and Padding = 1               | 1.1636     | 74.47          | 1.2781          | 63.0                |


 # Usage

Clone the Repository in your local machine along with the dataset.

Run the Python notebooks.
