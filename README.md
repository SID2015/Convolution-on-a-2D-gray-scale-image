# Convolution-on-a-2D-gray-scale-image

Let's explore how convolutions work by creating a basic convolution on a 2D Grey Scale image. 

1) We can load the image by taking the 'ascent' image from scipy. It's a nice, built-in picture with lots of angles and lines.

2) Next, we can use the pyplot library to draw the image so we know what it looks like.

3)The image is stored as a numpy array, so we can create the transformed image by just copying that array. Let's also get the dimensions of the image so we can loop over it later.

4)Now we can create a filter as a 3x3 array.

5)Now let's create a convolution. We will iterate over the image, leaving a 1 pixel margin, and multiply out each of the neighbors of the current pixel by the value defined in the filter.

i.e. the current pixel's neighbor above it and to the left will be multiplied by the top left item in the filter etc. etc. We'll then multiply the result by the weight, and then ensure the result is in the range 0-255

Finally we'll load the new value into the transformed image.

6)Now we can plot the image to see the effect of the convolution!

7)The code will show a (2, 2) pooling. The idea here is to iterate over the image, and look at the pixel and it's immediate neighbors to the right, beneath, and right-beneath. Taking the largest of them and load it into the new image. Thus the new image will be 1/4 the size of the old -- with the dimensions on X and Y being halved by this process. We'll see that the features get maintained despite this compression!


Please check the Attatched Screenshot

![](/imgs/img1.png)


![](/imgs/img2.png)


![](/imgs/img3.png)


![](/imgs/img4.png)
