# Object-Detection

Objection Detection can be categorised into 2 types
1. Region based Detectors and 2. One shot Detectors

**Object Detection Challenges:**
FCN's are widely used in image classification.
FCN's are challenged in object detection as the length of the output layer is a variable. This is because the number of ocvurences of the objects of interest are not fixed.
The use of sliding window of stride 1 would slow down the operation
So, one way of solving this would be to partition the input image into several regions and use a CNN to classify the presence of the object within each region.

**Drawbacks:**
The objects of interest might have Different spatial locations within the image and different aspect ratios.

Thus leaking out of the pre-set regions. To improve this naive approach one would need to select a very large number of regions(overlapping) which would increase the computational overhead.

