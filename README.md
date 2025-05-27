Download link : https://programming.engineering/product/com-sgn-110-exercise-4/

COM-SGN.110-EXERCISE 4
The tasks should be completed and presented to TA during the lab session. Do not forget to upload your solutions to Moodle! Questions about exercises should be addressed to the TA personally, through Moodle messages or via email, which can be found on the Moodle page of the course.

1. Image Enhancement Intensity Transformations

The focus of this part is to experiment with intensity transformations to enhance an image.

Download the image university.png and enhance it using:

(a) The log transformation

    = c log(1 + r) ,

Where c is a constant and it is assumed that r 0 . We would use a transformation of this type to expand the values of dark pixels in an image while compressing the higher-level values.

(b) a power-law transformation of the form

s = cr ,

Where c and γ are positive constants.

In (a) the only free parameter is c, but in (b) there are two parameters, c and γ for which values must be selected. As in most enhancement tasks, experimentation is a must. The objective of this exercise is to obtain the best visual enhancement possible with the methods in (a) and (b).

Once (according to your judgment) you have the best visual result for each transformation, explain the reasons for the major differences between them.

    Histogram Equalization

Implement your own histogram equalization function in a file histequal.m. Perform histogram equalization on the images (moon.png, house.png, spine.jpg, church.png) by your OWN method. Compare the histograms and images before and after processing. (for loops are allowed. Do not use MATLAB histeq function). Compare outputs to the ContrastStretch results (MATLAB code for ContrastStretch is provided).

    Histogram Matching

Implement your own function that applies histogram matching to an input image A such that the histogram of the output approximately matches the histogram of a reference image B. You can use simple interpolation, if necessary, but avoid using the built-in imhistmatch function. (see https://en.wikipedia.org/wiki/Histogram_matching)

Use spine.jpg or church.png as the input image A and corel.png as the reference image B. What can you observe?

    Properties of Histogram Equalization

        Explain in your own words why applying histogram equalization multiple times will have no additional effect.

        The histogram equalization gives results of varying quality for different images from Question 2. Explain why (hint: consider the original histograms). Can you now propose a way to improve the results for moon.png and spine.jpg, while still using histogram equalization?



