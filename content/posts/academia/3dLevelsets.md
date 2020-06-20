---
title: "A one-to-one Concrete Sample Computational Avatar"
subtitle: "from 3DXRCT images to a complete multi-phase computational model"
date: "2017-07-11"
draft: false
---

### About this project

![Characterization](/concrete.png)

From a real concrete sample, we extract 3DXRCT images from which we isolate the aggregate pixels. First, by processing the CT images and then by transforming the aggregates into scalar mathematical functions called Level-Sets. Once we have reconstructed the concrete cylinder using the aggregate Level-Sets we are ready to make a uniaxial computational simulation and compare it with the real concrete cylinder test. These is how fairly well processed images look like, these is actually a concrete cylinder.

After processing the 3DXRCT images and identifying the aggregates of the concrete mix, we proceed to evolve a surface towards the frontiers of the grain by using level sets. Level-set are scalar mathematical functions that implicitly determine the boundaries of the grain. Being the distance or level 0 the surface of the grain, outside it will be positive level or distance while inside it will be negative level or distance.

![Characterization](/levelset.png)

Finally, an example of a 3D level-set evolution towards the aggregate inside the concrete cylinder is shown.These digital avatars have an exact counterpart in the real life.

![Characterization](/levelsetProcess.gif)

Then a 2D Level-Set evolution is performed in order to transform the 3DXRCT grain images into mathematical functions, ready to be used in computerized granular models. We show a Level-Set evolution from a circular Level-Set function, in other words the initial guess is a circle. This evolution is guided or attracted basically by large image gradients. As you can see, the image gradient will be greater in the void-grain transition.

Finally, we show a Level-Set evolution given an initial binary grain solution. It is much faster and smoother!

![Characterization](/2dlevelset.gif)

## Project video

Short video about the image processing and later level set evoulution of the aggregates inside the sample. This video is more instructive rather than purely academic.

{{< youtube  "aN40k7PO5ZI" >}}
