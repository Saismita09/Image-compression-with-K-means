# Image-compression-with-K-means
In a straightforward 24-bit color representation of an image, each pixel is represented as three 8-bit unsigned integers (ranging from 0 to 255) that specify the red, green and blue intensity values. This encoding is often refered to as the RGB encoding. Our image contains thousands of colors, and in this project, I reduced the number of colors to 16 colors. By making this reduction, it is possible to represent (compress) the photo in an efficient way. Specifically, you only need to store the RGB values of the 16 selected colors, and for each pixel in the image you now need to only store the index of the color at that location (where only 4 bits are necessary to represent 16 possibilities). I treated every pixel in the original image as a data example and used the K-means algorithm to find the 16 colors that best group (cluster) the pixels in the 3-dimensional RGB space.

The resultant output obtained for sample image:
![](output.gif)
