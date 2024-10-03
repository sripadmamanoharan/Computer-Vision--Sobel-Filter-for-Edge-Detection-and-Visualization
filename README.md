# Computer-Vision--Sobel-Filter-for-Edge-Detection-and-Visualization

To implement a Sobel filter that computes the gradient of an image along the x and y directions. The Sobel filter will produce the gradient magnitude and orientation for each pixel. After normalizing the gradients to lie between [0,1], the results will be visualized using the HSV color space. In this visualization, the magnitude will determine the saturation and value (brightness), while the orientation will determine the hue. This technique helps in visualizing both the strength and direction of edges in an image.
Analysis Sobel Filter
– The Sobel filter is a popular edge-detection operator that calculates the gradient of the image in both the x and y directions.
– The gradient magnitude is computed as:
magnitude = qG2x + G2y
where Gx and Gy are the gradients in the x and y directions, respectively.
– The orientation of the gradient (in radians) is calculated as:
Gy  orientation = arctan Gx
Normalization
After calculating the gradient magnitude, the values are normalized to lie between [0, 1], making them suitable for visualization.
HSV Visualization
– The gradient magnitude is used to set the saturation and value (brightness) in the HSV color space.
– The orientation of the gradient is used to set the hue, which defines the color in the HSV space.
– This mapping allows us to visualize edges in color, where the intensity of the color reflects the strength of the edge, and the color itself reflects the direction of the edge.
Observation
– By mapping the gradient magnitude and orientation to the HSV color space, we can easily visualize both the strength and direction of edges.
– Strong edges are represented by bright, saturated colors, while weaker edges appear with dimmer or less saturated colors.
– The hue varies based on the edge direction, offering a clear representation of the edge orien- tation.
 8
Results and Observations
– The Sobel filter successfully detects the edges in the image, highlighting regions where the intensity changes significantly.
– Magnitude: The brighter and more saturated the color, the stronger the edge.
– Orientation: The hue changes with the direction of the edge, providing a clear representation
of the edge orientation.
Failure Cases
– Noise Sensitivity: If the image contains noise, the Sobel filter may detect false edges or amplify the noise, making the edge map cluttered.
– Low Contrast: In low contrast images, the edges may not be as distinct, making the detection less effective.
– High-Frequency Sensitivity: The Sobel filter can be sensitive to high-frequency compo- nents, which could lead to the detection of unwanted details or noise in the image.
