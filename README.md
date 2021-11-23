# Vanilla-Unet

![u-net-architecture](https://user-images.githubusercontent.com/87579053/142975359-04028f04-2c2f-4792-9888-431391f7bc7f.png)

The network consists of a contracting
path and an expansive path. The contracting path consists of the repeated
application of two 3x3 convolutions, each followed by activation function and a 2x2 max pooling operation
for downsampling. At each downsampling step we double the number of feature
channels. Every step in the expansive path consists of an upsampling of the
feature map followed by a convolution that halves the 
number of feature channels, a concatenation with the correspondingly 
feature map from the contracting path using skip connections. The final layer generates the segmentation mask for the given image.

### Dataset

The data on which unet was used is eye retina dataset.
![samples](https://user-images.githubusercontent.com/87579053/142975773-8edef9c8-3645-4362-9bc4-8d22f788252b.png)
