# Object_Localization_SIFT_Homography

The above repository corresponds to an assignment for the course Advanced Computer Vision by Prof. Ram Nevatia at USC

There are three source images and two destination images - the destination images contain the source images within them and the main task is to search for the source images in the destination images.

The code performs SIFT feature extraction on the source and the destination images, performs KNN matches on the keypoints, refines those matches, computes the homography matrix H using RANSAC via the refined (valid) matches (if the number of refined/valid matches is greater than some threshold, if not, no match between source and destination image is returned) and then uses the homography matrix to generate a bounding box (affine) of the source image within the destination image - this happens for all non-trivial (source, destination) combination.

The code isn't general and has been written to perform said task on the HW3_Data file images - though the code can be modified to perform a specific task or a task involving more images.

The code, once downloaded and run (assuming that the user has the relevant libraries), will generate folders with files for visualization - simply download the data and the notebook and run the notebook using the instructions in the read_me.txt file.

Reach out to me if there are any issues!

(Report can add more clarity to the task performed)
