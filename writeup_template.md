# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 

* I use ``select_line_color`` to keep yellow and white color in the image and remove other colors because the color of lines on 
the road is yellow or white

* Then change the images to grayscale

* Use ``region_of_interest`` to keep information in a specific area

* Use ``hough_lines`` to find lines in the image 

* Use ``generate_two_lines`` to find 2 lines, one in the left and the other in the right


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
