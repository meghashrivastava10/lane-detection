# lane-detection
This repository consists code for lane detection. 

The lane detection is implemented using OpenCV on a test video. For the lane detection the process followed is: 

    * Loading the Image: The test image is uploaded and the further scaling, edge detection, optimization is       implemented on the image. 
    * Grayscale: Converting the image into grayscale. This helps in increasing the contrast of lanes with respect to the road. 
    * Smoothening: Smoothening is done to enhance the image. The Gaussioan blur reduces the noise in the image.  
    * Edge Detection: The edge detection is performed to trace the strongest gradients. The gradient image traces the outline of the edges.
    * Region of Interest: The region of interest limits the extent of the field which ultimately traces the required part, here it is the triangle. 
    * Hough Transform: The Hough Transform is the technique used to detect any shape that can be represented mathematically. Here, we have displayed the lines on the required track that identifies the lane lines. 
    * Optimization: The optimization of the lane lines is done to identify the track more accurately.The multiple lines which are traced on the track is replaced by the single thus making the lane detection more accurate. 
    * Finding lanes on test video: Identified the line on the test video and executed the code to track the lanes. 

    We converted our color image into a gradient image and from the gradient image we detected the modet relevant lines, averaged out the lines and then displayed them on. The same procedure is applied on the test video and the lane detection on test is successfully implemented. 