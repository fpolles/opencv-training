# Description 
This repository contains Jupyter notebooks exploring image and video manipulation techniques using OpenCV.

- **PlayWithImage.ipynb** explores the following image processing techniques (single images, not video):
  - color manipulation
  - masking (selective image enhancement)
  - filtering (modifying pixel values)
 
- **PlayWithVideo.ipynb** explores the following video processing techniques:
  - filtering (modifying pixel values)
  - corner detection in video frames using `cv2.goodFeaturesToTrack`.\
    **Note:** Corner detection works well on textured surfaces like sand, which contain many well-defined edges. It is less effective on smooth regions like the open sea, resulting in fewer detected corners there.

- **PlayWithOpticalFlow.ipynb** extends the video processing work from `PlayWithVideo.ipynb` by introducing motion estimation. Covers two optical flow techniques and a color-based ball tracker:
  - Sparse Optical Flow (Lucas-Kanade): tracks corner features in the image.\
    **Note:** Lucas–Kanade relies on corner detection, so it naturally latches onto textured regions (e.g. flowers, foliage) and ignores smooth objects like balls that have no detectable corners.
  - Ball Tracking (HSV Masking + Contours): detects and tracks a ball based on its color using HSV thresholding and contour extraction
  - Dense Optical Flow (Farneback): estimates motion for all pixels in the frame, producing a dense motion field.
 
## Output Files
All outputs are saved to the `outputs/` folder.
    
## Libraries
These notebooks require [Python](https://www.python.org/) 3.14 and the following libraries:
- [NumPy](https://numpy.org/) 2.4
- [OpenCV](https://opencv.org/) 4.13
- [Matplotlib](https://matplotlib.org/) 3.10
