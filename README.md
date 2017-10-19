# AI-DNN-Papers
Papers on AI and DNNs

- [ ] https://arxiv.org/pdf/1703.07511.pdf

- [ ] https://arxiv.org/pdf/1703.06870.pdf

- [ ] https://arxiv.org/pdf/1612.07695v1.pdf

- [ ] https://arxiv.org/pdf/1612.08242.pdf

- [ ] http://papers.nips.cc/paper/5539-tree-structured-gaussian-process-approximations.pdf

- [ ] https://arxiv.org/pdf/1608.04062v1.pdf

- [ ] https://arxiv.org/pdf/1609.09365.pdf

- [ ] https://arxiv.org/pdf/1610.02242.pdf

- [ ] https://arxiv.org/pdf/1604.07316.pdf

- [ ] https://arxiv.org/pdf/1312.5602.pdf

- [ ] https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf

- [ ] https://arxiv.org/pdf/1404.7828.pdf

- [ ] http://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf

- [ ] https://arxiv.org/pdf/1606.03498.pdf

- [ ] https://arxiv.org/pdf/1703.03864.pdf

- [ ] https://openreview.net/forum?id=BJ0Ee8cxx

- [ ] https://openreview.net/forum?id=HkLXCE9lx

- [ ] https://openreview.net/forum?id=SJAr0QFxe

- [ ] https://openreview.net/forum?id=rJRhzzKxl

- [ ] https://openreview.net/pdf?id=ByldLrqlx

- [ ] http://www.chongyangma.com/publications/ld/2017_ld_preprint.pdf

- [ ] https://arxiv.org/pdf/1704.02399.pdf

- [ ] https://arxiv.org/pdf/1703.10593.pdf

- [ ] https://arxiv.org/pdf/1703.05192.pdf

- [ ] https://papers.nips.cc/paper/3311-hippocampal-contributions-to-control-the-third-way.pdf

- [ ] https://arxiv.org/pdf/1605.06065.pdf

- [ ] https://arxiv.org/pdf/1704.05519.pdf

- [ ] [Deep Learning Survey](https://www.nature.com/articles/nature14539.epdf?referrer_access_token=K4awZz78b5Yn2_AoPV_4Y9RgN0jAjWel9jnR3ZoTv0PU8PImtLRceRBJ32CtadUBVOwHuxbf2QgphMCsA6eTOw64kccq9ihWSKdxZpGPn2fn3B_8bxaYh0svGFqgRLgaiyW6CBFAb3Fpm6GbL8a_TtQQDWKuhD1XKh_wxLReRpGbR_NdccoaiKP5xvzbV-x7b_7Y64ZSpqG6kmfwS6Q1rw%3D%3D&tracking_referrer=www.nature.com)

- [ ] https://arxiv.org/pdf/1409.3215.pdf

- [ ] https://arxiv.org/pdf/1502.03167.pdf

- [ ] https://arxiv.org/pdf/1502.01852v1.pdf

- [ ] https://arxiv.org/pdf/1312.6229v4.pdf

- [ ] http://www.cs.toronto.edu/~hinton/absps/imagenet.pdf

- [ ] https://arxiv.org/pdf/1610.05755.pdf

- [ ] https://arxiv.org/pdf/1703.10631.pdf

- [ ] https://arxiv.org/pdf/1705.01389.pdf

- [ ] https://arxiv.org/abs/1703.07326.pdf

- [x] https://research.fb.com/wp-content/uploads/2017/06/imagenet1kin1h3.pdf?

  - Presents an approach using linear scaling of learning rates based on batch size (**RULE:** When minibatch size is scaled by _k_, scale the learning rate by _k_ where k is the number of nodes in the cluster) and a "warmup" period at the beginning of training using a low learning rate to avoid initial optimization difficulties thereby allowing the use of large batch sizes in training, leading to equivilent generalization accuracy as well as matching training curves in a fraction of the time for ImageNet Classification with ResNet  
- [ ] https://arxiv.org/pdf/1704.00051.pdf

- [ ] https://arxiv.org/pdf/1705.07204.pdf

- [ ] https://arxiv.org/pdf/1707.06728.pdf

- [ ] https://arxiv.org/pdf/1704.01155.pdf

- [X] https://arxiv.org/pdf/1703.06211v3

  - Introduces the concepts of Deformable Convolutions and Deformable Region of Interest (RoI) Pooling. Both can be dropped in place of standard components in current CNNs, and can be trained with standard back propogation. Standard convolutions are fixed geometrically and so require large ammounts of training or complex model parameters to learn robust representations. Other fixed techniques like SIFT and sliding window rely on tranformation invariant features. Convolution's modeling capablity comes from large amounts of data augmentation and additional hand crafted components like max pooling to address small translation invariance. CNNs are limited to large transformations due to the fixed geometric structure of the modules e.g. Max Pooling reduces the resolution by a fixed ammount or RoI createsfixed bins. The paper introduces a new set of learned parameters for convolutional layers that correspond to offsets from the regular grid sampling locations. The offsets are learned by the feature maps in the preivious layers, via additional convolution layers. Deformable RoI Pooling addes an offset to the normal bin partition of the preivous pooling layer. These offsets are also learned. Deformable Convolution has 2 steps. 1. samples using the regular grid augmented with the trained offsets over the input feature map 2. sampled values are summed and weighted. To learn the offsets, gradients are backproped. Deformable RoI takes a input feature map and a dRoI of size _w_x_h_ and a top left corner and splits the RoI into _k_x_k_ bins each offset from the RoI bin position by a learned offset. The output feature map is the collection of bins created by the dRoI. The offsets are learned via a fully connected layer which applies the offsets on a standard RoI.  
  
  - Terms to Look into:
    - Bilinear Interpolation
    - Spatial Transform Networks
    - Active Convolution
    - Effective Receptive Field
    - Deformable Part Models 
    - Artous Convolution -> Increase filter stride, sparsifies sampling  
    
- [ ] https://arxiv.org/pdf/1612.01105

- [ ] https://arxiv.org/pdf/1611.09842

- [ ] https://arxiv.org/pdf/1703.10593

    - Presents a method for image to image translation without paired examples.
Does This by learning the key characteristics of a set X and a set Y and then
tries to develop a translation function to apply the key characteristics. Trains
the GAN using a cycle consistancy loss (f(g(X)) -> X) and an adversarial loss.

- [ ] https://arxiv.org/pdf/1705.07115.pdf

### Sites and Links
https://openai.com/blog/universe/

http://www.scholarpedia.org/article/Neuroevolution

https://blog.openai.com/evolution-strategies/

http://arxiv-sanity.com/

https://github.com/hindupuravinash/the-gan-zoo

https://bigredt.github.io/2017/07/09/reason/

http://luthuli.cs.uiuc.edu/~daf/courses/LearningCourse17/learning-book-Mar-17-all-small.pdf
