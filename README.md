# detect-circles-using-opencv
- I have imported opencv and numpy libraries
- used cv2.imread to read the image
- converted the image to grayscale
- used median filter on grayscale image to remove noise
- then again converted grayscale image to rgb
- Then I have used hough circle algorithm to detect circles.
- It has some parameters in it which are
- input image 
- method (in my case i have used cv2.HOUGH_GRADIENT
- dp (inverse ratio of the accumulator resolution to the image resolution. For example, if dp = 1 , the accumulator has the same resolution as the input image. If dp = 2   the accumulator has half as big width and height.)
- minDist (	minimum distance between the centers of the detected circles. If the parameter is too small, multiple neighbor circles may be falsely detected in addition to a true one. If it is too large, some circles may be missed)
- param1 (it is sensitivity of circle detection if it is too high it is not going to detect any circles and if it is too low it will find too many circles)
- param2 ( accuracy of circle detection it sets the no of edge points that are needed to declare that there is a circle again if it is set too high it will detect no circle and if it is set too low it will set too many circles)
-min radius  minimum size of circle that can be detected
-max radius  
- convert circles to a numpy array
- Draw the outer circle and inner circle using cv2.circle again we have to fill the parameters which are
-image name
- center point of circle
- radius 
- color of circle
- thickness
- lastly i used cv2.imshow to print out the resultant image after applying hough transform

