Used in [[canny edge detection]] to reduce image noise. Essentially, take an $n\times n$ region of an image, and plot those pixel images against some gaussian distribution.

The filter returns an average value of those $n\times n$ pixels, but the average is weighted towards the center of the distribution (i.e. values within 1 s.d. are weighted more). 