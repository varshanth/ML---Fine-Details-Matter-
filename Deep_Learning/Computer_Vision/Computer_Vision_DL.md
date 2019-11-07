# Deep Learning: Computer Vision
These resources are not mine and I do not claim that I have written/composed/presented them. They are an aggregation of publicly available resources. If any of the authors do not want their resources cited here, please report it as an issue and I will remove it from the repo at the earliest.  

* CS231n Lec 11 - Semantic Segmentation, Classification + Localization, Object Detection  

## Revolutionary CNN Architectures
* CS231n Lec 9 - CNN Architectures - VGGNet, GoogLeNet, ResNet, etc.
* A brief about ResNets and its variants:  
https://towardsdatascience.com/an-overview-of-resnet-and-its-variants-5281e2f56035
* ResNet Paper by He et al.  
https://arxiv.org/pdf/1512.03385.pdf  
CVPR 2016 ResNet Presentation: https://www.youtube.com/watch?v=C6tLw-rPQ2o
* DenseNet Paper by Huang et al.  
https://arxiv.org/pdf/1608.06993.pdf  
DenseNet - (L) Meaning:  
https://github.com/liuzhuang13/DenseNetCaffe/issues/9  
CVPR 2017 DenseNet Presentation: https://www.youtube.com/watch?v=xVhD2OBqoyg
* Dual Path Networks by Chen et al.  
https://arxiv.org/pdf/1707.01629.pdf

### Global Average Pooling

* Why is Global Average Pooling replacing FC Layers nowadays?  
https://www.quora.com/What-is-global-average-pooling  
* Very brief simple explanation of what GAP is:  
https://stats.stackexchange.com/questions/257321/what-is-global-max-pooling-layer-and-what-is-its-advantage-over-maxpooling-layer  
* Origination & Concept Proposal by Lin et al.  
https://arxiv.org/pdf/1312.4400.pdf  
  
## Architectural Innovations for Compressing CNNs

* Overview:  
https://medium.com/@nicolas_19145/state-of-the-art-in-compressing-deep-convolutional-neural-networks-cfd8c5404f22  
* SqueezeNet Code:  
https://github.com/gsp-27/pytorch_Squeezenet/blob/master/model.py  
* MobileNet Explained:  
http://machinethink.net/blog/googles-mobile-net-architecture-on-iphone/  
* MobileNet v2 Explained:  
http://machinethink.net/blog/mobilenet-v2/  
https://towardsdatascience.com/mobilenetv2-inverted-residuals-and-linear-bottlenecks-8a4362f4ffd5  
* ShuffleNet Explained:  
https://medium.com/syncedreview/shufflenet-an-extremely-efficient-convolutional-neural-network-for-mobile-devices-72c6f5b01651  
Code:  
https://www.youtube.com/watch?v=pNuBdj53Hbc

## Object Detection
* Succinct Explanations:  
https://leonardoaraujosantos.gitbooks.io/artificial-inteligence/content/object_localization_and_detection.html  
* IoU Explained:  
https://www.pyimagesearch.com/2016/11/07/intersection-over-union-iou-for-object-detection/  
* Summaries with Mathematical Explanations:  
https://lilianweng.github.io/lil-log/2017/12/31/object-recognition-for-dummies-part-3.html  
https://lilianweng.github.io/lil-log/2018/12/27/object-detection-part-4.html  

### Evaluation Metric: mean Average Precision (mAP)  
* Read until (excluding) Interpolated Precision [Their toy example is wrong]:  
https://towardsdatascience.com/breaking-down-mean-average-precision-map-ae462f623a52
* Should make things crystal clear:  
https://medium.com/@jonathan_hui/map-mean-average-precision-for-object-detection-45c121a31173  
* Good visualization of PR curves because all the above toy examples give the ideal scenario when recall of 1.0 can actually be achieved. This will give a good visualization of realistic recall values at higher IoU thresholds:  
https://medium.com/@timothycarlen/understanding-the-map-evaluation-metric-for-object-detection-a07fe6962cf3  

In summary:

1) Take predictions of a certain class  
2) Filter out the predictions lower than the IoU threshold "T"  
3) Sort the remaining predictions in descending order of the class confidence (softmax) values  
4) Calculate the AP  
5) Perform Steps 1) to 4) for all classes  
6) Take average across all classes to get the mAP@T  

### Faster RCNN
* Faster RCNN (FRCNN) Level 1 Detailed Explanation:  
https://tryolabs.com/blog/2018/01/18/faster-r-cnn-down-the-rabbit-hole-of-modern-object-detection/  
* FRCNN Level 2 Detailed Explanation:  
http://www.telesens.co/2018/03/11/object-detection-and-classification-using-r-cnns/  
For the same link with my comments: Check [this](Faster_RCNN_Explained.pdf)
* L1 Loss for BBox Regression:  
https://mohitjainweb.files.wordpress.com/2018/03/smoothl1loss.pdf  
* Anchor Box Seeding (used in SSD and YOLO too):  
https://lars76.github.io/object-detection/k-means-anchor-boxes/  
* Region of Interest (RoI) Pooling:  
https://blog.deepsense.ai/region-of-interest-pooling-explained/  

### SSD

* https://medium.com/@smallfishbigsea/understand-ssd-and-implement-your-own-caa3232cd6ad  
* https://medium.com/@jonathan_hui/ssd-object-detection-single-shot-multibox-detector-for-real-time-processing-9bd8deac0e06  
* https://towardsdatascience.com/review-ssd-single-shot-detector-object-detection-851a94607d11
* http://www.telesens.co/2018/06/28/data-augmentation-in-ssd/#Data_Augmentation_Steps

### RetinaNet

* https://towardsdatascience.com/review-retinanet-focal-loss-object-detection-38fba6afabe4  
