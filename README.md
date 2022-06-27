# U-Shape-Based-Architecture-with-Adjusted-Bilateral-Guided-Aggregation-Layer-for-Nuclei-Image-Segment
## Introduction
Cell Segmentation on the dataset [Data Science Bowl](https://www.kaggle.com/c/data-science-bowl-2018)
## Our contributions
![abga](https://github.com/tswizzle141/U-Shape-Based-Architecture-with-Adjusted-Bilateral-Guided-Aggregation-Layer-for-Nuclei-Image-Segment/blob/main/1.jpg)
![proposed-model](https://github.com/tswizzle141/U-Shape-Based-Architecture-with-Adjusted-Bilateral-Guided-Aggregation-Layer-for-Nuclei-Image-Segment/blob/main/2.jpg)
* We replaced the skip connection between encoder and decoder blocks with Adjusted Bilateral Guided Aggregation (ABGA) layer. We select several intermediate outputs in the pre-trained EfficientNet-B4 architecture as connecting components between encoder and decoder branches. In specific, outputs of layers 342nd, 154th, 143rd and 85th are selected owing to their moderate amount of parameters and their position as batch normalization layers.Corresponding feature maps from the two blocks are aggregated by Adjusted Bilateral Guided Aggregation Layer as follows. 
* Our proposed loss function is simply retrieved by subtracting Kulczycki 2 coefficient which takes the form:
$$\mathcal{K}= 1 - Kulc = 1 - \dfrac{1}{2}\left(\dfrac{TP}{TP + FN} + \dfrac{TP}{TP + FP} \right)$$
## Results
![table1](https://github.com/tswizzle141/U-Shape-Based-Architecture-with-Adjusted-Bilateral-Guided-Aggregation-Layer-for-Nuclei-Image-Segment/blob/main/3.jpg)
![table2](https://github.com/tswizzle141/U-Shape-Based-Architecture-with-Adjusted-Bilateral-Guided-Aggregation-Layer-for-Nuclei-Image-Segment/blob/main/4.jpg)
