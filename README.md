# Finding Lane Lines on the Road

[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.


Submission
---

This project is my (Andrei Bârsan) solution to this first assignment. I took it
as part of a free preview of the course.

The solution uses a moderate Gaussian blur, a canny edge detector, and a Hough
transform for detecting line segments. The system then merges the raw line
segments into full lane limits using RANSAC. The results are also smoothed over
a few frames to remove jitter and increase robustness.

More details about the implementation are present in the project writeup,
`writeup.md`.

The code is written in Python 3, and uses Jupyter, OpenCV, and a little bit of
scikit-learn.  All the logic is located in the `P1.ipynb` notebook.
