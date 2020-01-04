# **Finding Lane Lines on the Road** 

### Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on the work in a written report

### Reflection

### 1. Describe your pipeline. 

My pipeline consisted of 5 steps. 

* I use ``select_line_color`` to keep yellow and white color in the image and remove other colors because the color of lines on 
the road is yellow or white

* Then change the images to grayscale

* Use ``region_of_interest`` to keep information in a specific area

* Use ``hough_lines`` to find lines in the image 

* Use ``generate_two_lines`` to find 2 lines, one in the left and the other in the right

The flow chart image processing
![Graph](https://github.com/ms5898/CarND-LaneLines-P1/blob/master/examples/flow_chart.png)


### 2. Identify potential shortcomings with your current pipeline

* This method does not perform well when road lines are short or not obvious

* When processing ``challenge.mp4`` Sometimes yellow stains or tree shadows on the ground can affect the output

### 3. Suggest possible improvements to your pipeline

* Add memory so that when the marker line disappears, you can use the previous results to predict the route

* Add function to identify between road markings and noise
