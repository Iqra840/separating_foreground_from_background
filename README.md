# separating_foreground_from_background
Program that isolates foreground(usually the user) from the background in a video

Utilizing the methods in OpenCV, this code spearates the foreground from the background of a video by first converting it to grayscale and detecting on edges based on a certain threshold (that can be adjusted for the user's requirement). Thresholds are also set for the maximum area and minimum area a contour within a frams can occupy for it to be in the foreground. Dilation and erosion further fine tune the edges and a mask is then created from the computations which, when merged with the image, give the foreground as an isolated image. The user can use this result to set up a virtual background on Zoom, which constitutes part 2 of this project.
