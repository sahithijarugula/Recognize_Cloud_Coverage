# Recognizing Cloud Coverage in Images of the Sky
## Introduction
Cloud coverage is an important element in understanding the earth’s atmosphere and predicting the weather. There are multiple research topics that cloud coverage impacts. For example, clouds can reduce and block the penetration of solar radiation and monitoring cloud coverage can improve scientists’ knowledge on radiation patterns. An accurate and efficient cloud coverage classification system can largely speed up the process of  future research on such topics. In this project, we compared different machine learning methods that automate the detection of cloud coverage in images of the sky, in an attempt  to develop a  classification system that can be of use to other scientists.  
## Dataset
NASA GLOBE Cloud: this dataset provides images of the sky taken by citizens from the ground along with associated metadata such as cloud cover. We collected 120 images (20 for each cloud coverage category– none, mostly clear, isolated, scattered, broken, and overcast) to test our cloud coverage classification  methods.
## Methods
Saturation Thresholding: uses the HSV version of an image1 to distinguish the difference between cloud and sky pixels.
CLAHE  Thresholding: uses Contrast Limited Adaptive Histogram Equalization to enhance differences between cloud and sky pixels.
Blue Channel  Thresholding: uses the blue channel of an image and adaptive thresholding to separate cloud and sky pixels in an image.
Hybrid Thresholding: Combination of the Saturation (used for scattered, isolated and  broken images), CLAHE (used for overcast images), and Blue Channel (used for none and mostly clear images) thresholding methods
Morphological Snakes: Image Processing method that utilizes image contours2 in order to separate background and foreground.

