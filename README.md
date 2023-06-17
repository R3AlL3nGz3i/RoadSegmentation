# RoadSegmentation

This project uses Unet to perform segmentic segmentation of the road in order to enhanced Mapping and Localization.
The network architecture started with an encoder followed by a decoder paths. 
As usual, the encoder path contains three main layers, convolutional layer, max pooling layer to downsampling the input image the and a dropout layer while a 
decoder path contains upsampling and convolutional layer. The upsampling was done by concatenating the downsampling and upsampling path, often we called it as
skip connection will help to  preserve fine-grained spatial information. It allows the free flow of gradients through skip connection to mitigate vanishing gradients.  
![download](https://github.com/R3AlL3nGz3i/RoadSegmentation/assets/85697619/b8b5b996-0b32-4471-b5fc-6e77aecb2585)
