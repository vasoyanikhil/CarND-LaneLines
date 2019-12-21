# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Test pipeline using images
* Test pipeline using video

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps As I mention below.

1. I converted the images to grayscale.

2. I apply Canny to the gray image then output of the image called edges. Apply high and low thresholds for edge detection.

3. I apply region of the interest which region needed to mask.

4. I apply Hough transform on mask image then I got output list of the lines after classify lines as left and right.After take average of all left lines and all right lines then draw the left and right line. 

5. After getting the line images to combine with original images. 


<img src= "https://github.com/vasoyanikhil/UDACITY/blob/master/CarND-LaneLines-P1/test_images_output/solidWhiteCurve.jpg" >

### 2. Identify potential shortcomings with your current pipeline

I try in this project in Optional Challenge but I did not get output as I expected.

### 3. Suggest possible improvements to your pipeline

I need to modify the Draw_line function so I will get more accurate output of the optional Challenge video.
