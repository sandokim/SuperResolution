[Deep learning based Super Resolution](https://www.analyticsvidhya.com/blog/2021/05/deep-learning-for-image-super-resolution/)

<img src="https://github.com/sandokim/SuperResolution/blob/main/images/Pre-upsampling SR.png" width="80%">

<img src="https://github.com/sandokim/SuperResolution/blob/main/images/Post-upsampling SR.png" width="80%">

Learning Strategies
* Pixelwise L1 loss – Absolute difference between pixels of ground truth HR image and the generated one.
* Pixelwise L2 loss – Mean squared difference between pixels of ground truth HR image and the generated one.
* **Content loss** – the content loss is indicated as the **Euclidean distance between high-level representations of the output image and the target image.** High-level features are obtained by passing through pre-trained CNNs like VGG and ResNet.
* Adversarial loss – Based on GAN where we treat the SR model as a generator, and define an extra discriminator to judge whether the input image is generated or not.
* PSNR – Peak Signal-to-Noise Ratio (PSNR) is a commonly used objective metric to measure the reconstruction quality of a lossy transformation. PSNR is inversely proportional to the logarithm of the Mean Squared Error (MSE) between the ground truth image and the generated image.
