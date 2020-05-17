---
title: "Image processing"
subtitle: "From granular 3DXRCT images to a 2D level set evolution"
date: "2017-07-11"
draft: false
---

### About this project

![Characterization](/jamSlice.png)

From a real granular sample we extract 3DXRCT images and then isolate the grains pixels. First, we process the CT images to further transform the grain pixels into scalar mathematical functions called Level-Sets.

The samples depicted are Jaramijó Secondary Lahars (Ecuador soil) and the respective 3D pixel reconstruction of those slices. However, the main problem with these slices is that they are raw images, therefore they are really noisy which makes really difficult to know what is a grain or empty space.

If we make zoom onto the images we will clearly see how noisy they are. First, we use a Non Local Means filter, which as its name states, it is non local meaning that it ponderates the neighboring image windows distance from the one being analyzed, in other words neighboring image windows that are far away from the actual image window are going to recibe less ponderation. Second, we binarize the slice in order to better distinguish what is a grain and what is void space using a classical Threshold Otsu method, which basically divides the area of the pixels histogram in two, this point of division is the actual threshold that tells us that below that threshold we have empty space and above that threshold we have a grain.

![Characterization](/processing.png)

Then a 2D Level-Set evolution is performed in order to transform the 3DXRCT grain images into mathematical functions, ready to be used in computerized granular models. We show a Level-Set evolution from a circular Level-Set function, in other words the initial guess is a circle. This evolution is guided or attracted basically by large image gradients. As you can see, the image gradient will be greater in the void-grain transition.

Finally, we show a Level-Set evolution given an initial binary grain solution. It is much faster and smoother!

![Characterization](/2dlevelset.gif)

## Project video

Short video about the image processing and later level set evoulution of grains inside the sample. This video is more instructive rather than purely academic.

{{< youtube  "_cuVQWQpRH8" >}}
