This folder contains all the results we have got from our trained pix2pix network. There are altogether 645 images from 256 different classes. Each image is of size 256 * 768 * 3, which is a concatenation of three 256 * 256 * 3 images. The left, middle, right image stands for the ground truth, the sketch generated by the cycleGAN network, and the reconstructed image generated by the pix2pix network. We collect all the test images instead of picking only a few of them, simlply because all of them are equally good and presenting all the images from different classes also reinforce the idea that pix2pix network is able to handle the image-to-image translation task in a general setting, even if the training data come from as large as 256 different categories. As we have discussed in our final report, the output images from the pix2pix network (right) are of less variation in color compared to the original images. Our result shows that monotonous coloring is pervalent among the generated images. 

As for the cycleGAN encoder which is responsible for generating fake sketches (middle) from original images (left), our results show that the cycleGAN encoder also performs well in general. It is able to convert an image to a sketch even if the image is from a distribution that is totally different from that in the training set, as we have discussed in our report. However, failure cases are also very common. We can see that the performance of cycle GAN gets worse when facing with color transition that it has never been presented before. triple_img_9.jpg  and triple_img_39.jpg are good examples where the cycle GAN performs terribly on sketching the insects' body, resulting in local blur in the reconstructed image.

Appendix:
10 among the 645 images I like best: 
1. alpaca (triple_img_4.jpg)
2. bush (triple_img_82.jpg)
3. church (triple_img_125.jpg)
4. crocodile (triple_img_151.jpg)
5. dragon (triple_img_173.jpg)
6. eye (triple_img_186.jpg)
7. monkey (triple_img_334.jpg)
8. revolver (triple_img_433.jpg)
9. space shuttle (triple_img_502.jpg)
10. train (triple_img_590.jpg)

Which one(s) do you like?
