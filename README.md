# Opencv_historgram
Use of Histogram for object/image matching

Two core OpenCV functions were used

cv2.calcHist(images, channels, mask, histSize, ranges) → hist
Parameters:
images – Source arrays. They all should have the same depth, CV_8U or CV_32F , and the
same size. Each of them can have an arbitrary number of channels.
channels – List of the dims channels used to compute the histogram.
mask – Optional mask. If the matrix is not empty, it must be an 8-bit array of the same size as
images[i] . The non-zero mask elements mark the array elements counted in the histogram.
histSize – Array of histogram sizes in each dimension.
ranges – Array of the dims arrays of the histogram bin boundaries in each dimension. Specify
the lower (inclusive) boundary of the histogram bin and the upper (exclusive) boundary. The
values for ranges and histSize must be compatible.

cv2.compareHist(H1, H2, method) → retval
Parameters:
H1 – histogram 1
H2 – histogram 2
method – comparison method
cv2.CV_COMP_CORREL Correlation
cv2.CV_COMP_CHISQR Chi-Square
cv2.CV_COMP_INTERSECT Intersection
cv2.CV_COMP_BHATTACHARYYA Bhattacharyya distance

Dataset-HistogramDataset
├── classes
│ ├── pikachu [10 entries]
│ ├── bulbasaur [10 entries]
│ ├── charmander [10 entries]
│ └── squirtle [10 entries]
├── targets [4 entries]
├── mystery [10 entries]
