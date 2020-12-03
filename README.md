# Opencv_historgram
Use of Histogram for object/image matching

Two core OpenCV functions were used

cv2.calcHist(images, channels, mask, histSize, ranges) → hist<br />
Parameters:<br />
images – Source arrays. They all should have the same depth, CV_8U or CV_32F , and the<br />
same size. Each of them can have an arbitrary number of channels.<br />
channels – List of the dims channels used to compute the histogram.<br />
mask – Optional mask. If the matrix is not empty, it must be an 8-bit array of the same size as<br />
images[i] . The non-zero mask elements mark the array elements counted in the histogram.<br />
histSize – Array of histogram sizes in each dimension.<br />
ranges – Array of the dims arrays of the histogram bin boundaries in each dimension. Specify
the lower (inclusive) boundary of the histogram bin and the upper (exclusive) boundary.<br />
values for ranges and histSize must be compatible.

cv2.compareHist(H1, H2, method) → retval<br />
Parameters:<br />
H1 – histogram 1<br />
H2 – histogram 2<br />
method – comparison method<br />
cv2.CV_COMP_CORREL Correlation<br />
cv2.CV_COMP_CHISQR Chi-Square<br />
cv2.CV_COMP_INTERSECT Intersection<br />
cv2.CV_COMP_BHATTACHARYYA Bhattacharyya distance<br />

Dataset-HistogramDataset<br />
1.classes<br />
  -pikachu [10 entries]<br />
  -bulbasaur [10 entries]<br />
  -charmander [10 entries]<br />
  -squirtle [10 entries]<br />
2.targets [4 entries]<br />
3.mystery [10 entries]<br />
