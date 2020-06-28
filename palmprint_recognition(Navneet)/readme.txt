Python Palmprint Recognition:

Palmprint recognition with SKimage and OpenCV

Requirements:
- NumPy
- SKimage
- OpenCV2


Works by extracting minutiae points using harris corner detection.

Uses SIFT (ORB) go get formal descriptors around the keypoints with brute-force hamming distance and then analyzes the returned matches using thresholds.

Usage:

1. Place 2 fingerprint images that you want to compare inside the database folder
2. Pass the names of the images as arguments in the console



Dockerfile:

docker build -t <name_of_your_choice> 

docker run -it <name_of_your_choice> <palmprint_1> <palmprint_2>

NOTE: The Palmprints must be in the `/database` folder

References:

1. https://github.com/ivonajdenkoska/fingerprint-recognition
2. https://www.peterkovesi.com/
