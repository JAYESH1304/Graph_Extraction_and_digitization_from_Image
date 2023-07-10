# Graph Extraction and Digitization from Image
This repository contains code for extracting a graph from an image using Python and OpenCV.

The graph() function takes an input image and performs the following steps to generate the graph:

1. Converts the image to grayscale.
2. Applies a threshold to create a binary image.
3. Finds contours in the binary image using the external retrieval mode.
4. Selects the contour with the maximum arc length.
5. Approximates the contour using the Douglas-Peucker algorithm.
6. Reshapes the approximation and extract the x-y coordinates.
7. Groups the y-coordinates based on their corresponding x-coordinates.
8. Calculates the average y-coordinate for each x-coordinate group.
9. Sorts the new points based on their x-coordinates.
10. Performs cubic interpolation on the new points.
11. Generates x and y arrays for plotting.
12. Adjusts the x-coordinates to start from zero.
13. Creates a cubic interpolation model using SciPy.
14. Generates interpolated values on a finer x-axis grid.
15. Plots the interpolated curve.
    
To use the function, provide an image containing a graph as the input and call the graph() function.





