# Semantic-Segmentation-basic-for-your-subject
A paper list of semantic segmentation using deep learning<br>
- [论文主要内容快速获取](#各论文主要内容快速获取)
- [论文网络性能表](#各论文网络性能表)
- [论文关注点及贡献](#各论文关注点及贡献)
## 各论文主要内容快速获取
   1. [FCN](FCN/README.md)
## 各论文网络性能表
|network|VOC12|VOC12 with COCO|Pascal Context|CamVid|Cityscapes|ADE20K|Published In |
|:-----:|:--------:|:------------------:|:-----------------:|:---------:|:-------------:|:---------:|:-----------:|
|FCN-8s |62.2      |                    |37.8               |           |65.3           |           |CVPR 2015    |
|DeepLab|71.6      |                    |                   |           |               |           |ICLR 2015    |
|CRF-RNN|72.0      |74.7                |39.3               |           |               |           |ICCV 2015    |
|DeconvNet|72.5    |                    |                   |           |               |           |ICCV 2015    |
|DPN    |74.1      |77.5                |                   |           |               |           |ICCV 2015    |
|SegNet |          |                    |                   |50.2       |               |           |
|Dilation8|        |75.3                |                   |           |               |           |
|Deeplab v2|       |79.7                |45.7               |           |70.4           |           |PAMI         |
|FRRN B |          |                    |                   |           |71.8           |           |CVPR 2017    |
|G-FRNet|79.3      |                    |                   |68.0       |               |           |CVPR 2017    |
|GCN|              |82.2                |                   |           |76.9           |           |CVPR 2017    |
|SegModel|         |82.5                |                   |           |79.2           |           |CVPR 2017    |
|RefineNet|        |83.4                |47.3               |           |73.6           |40.7       |CVPR 2017    |
|PSPNet|82.6       |85.4                |                   |           |80.2           |           |CVPR 2017    |
|DIS|              |86.8                |                   |           |               |           |ICCV 2017    |
|SAC-multiple|     |                    |                   |           |78.1           |44.3       |ICCV 2017    |
|DeepLabv3|        |85.7                |                   |           |81.3           |           |arxiv 1706.05587|
|DUC-HDC|          |                    |                   |           |80.1           |           |WACV2018|
|DDSC|81.2         |                    |47.8               |70.9       |               |           |CVPR 2018|
|EncNet|82.9       |85.9                |51.7               |           |               |44.65      |CVPR 2018|
|DFN|82.7          |86.2                |                   |           |80.3           |           |CVPR 2018|
|DenseASPP|        |                    |                   |           |80.6           |           |CVPR 2018|
|UperNet|          |                    |                   |           |               |42.66      |ECCV 2018|
|PSANet|           |85.7                |                   |           |80.1           |43.77      |ECCV 2018|
|DeepLabv3+|       |87.8                |                   |           |82.1           |           |ECCV 2018|
|ExFuse|           |87.9                |                   |           |               |           |ECCV 2018|
|OCNet|            |                    |                   |           |81.2(81.7)     |45.08(45.45)|arxiv 1809.00916|
|DAN|              |                    |52.6               |           |78.2           |           |CVPR 2019|
|DPC|              |87.9                |                   |           |82.7           |           |NIPS 2018|
|CCNet|            |                    |                   |           |81.4           |45.22      |arxiv 1811.11721|
|GloRe|            |                    |                   |           |80.9           |           |CVPR 2019|
|TKCN|             |83.2                |                   |           |79.5           |           |ICME 2019|
|GCU|              |                    |                   |           |               |44.81      |NIPS 2018|
|DUpsampling|85.3  |88.1                |52.5               |           |               |           |CVPR 2019|
|FastFCN|          |                    |53.1               |           |               |44.34      |arxiv 1903.11816|
|GFF|              |                    |                   |           |82.3           |45.33      |arxiv 1904.01803|
|HRNetV2|          |                    |54.0               |           |81.6           |           |arxiv 1904.04514|
|CaseNet|          |                    |                   |           |81.9           |45.28      |arxiv 1904.08170|

## 各论文关注点及贡献
|network|focus |contributions|
|:-----:|:-----------------:|:-----------------------------------------------------------------------------:|
|FCN    |improve performance|1. fully convolution layer<br>2. skip-architecture|
|UNet   |improve performance|1. augmentation(shift,rotation and gray value)<br>2. encoder-decoder construction(combine contract feature map and extend feature map)<br>3. weighted loss|
|DilatedNet|improve performance         |1. aggregates multi-scale contextual information without losing resolution|
|ENet   |real-time          |1. ENet initial block<br>2. ENet bottleneck module|
|PixelNet|improve performance|1. multi-scale sampling layer<br>2. sampling pixel to train|
|SegNet|real-time|1. max-pooling indices(replace the concatenation of feature maps between encoder and decoder)|
|PSPNet|improve performance|1. pyramid scene parsing network<br>2. auxiliary loss(for refine the learning process)|
|LinkNet|real-time|1. initial block(downsampling input)<br>2. encoder block(resnet block)<br>3. decoder block(bolttleneck block)|
|DeepLab(v1~v3+)|improve performance|1. CRF<br>2. dilated conv<br>3. ASPP combine with encoder-decoder<br>4. group conv|
|ICNet|improve performance|1. cascade input image<br>2. cascade label guidance for traning|

