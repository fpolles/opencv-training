# Description 
This repository contains notebooks exploring several image and video manipulation techniques using OpenCV.

- **PlayWithImage.ipynb** explores the following image processing techniques (single images, not video):
  - color manipulation
  - masking (selective image enhancement)
  - filtering (modifying pixel values)
 
- **PlayWithVideo.ipynb** explores the following video processing techniques:
  - filtering (modifying pixel values)
  - corner detection in video frames using `cv2.goodFeaturesToTrack`.

    **Note** In this exercise, corner detection works well for elements such as sand, which contain many clear, well-defined corners. It is less effective for smoother areas like the sea, resulting in fewer detected corners in those regions.

## Libraries
This notebook requires [Python](https://www.python.org/) 3.14 and the following libraries:
- [NumPy](https://numpy.org/) 2.4
- [OpenCV](https://opencv.org/) 4.13
- [Matplotlib](https://matplotlib.org/) 3.10
