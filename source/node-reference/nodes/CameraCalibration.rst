CameraCalibration
=================

**Description**

.. Note:: 
   This node requires AliceVision compiled with OpenCV.

The internal camera parameters can be calibrated from multiple views of a checkerboard. This allows to retrieve focal length, principal point and distortion parameters. A detailed explanation is presented in [opencvCameraCalibration].

[opencvCameraCalibration] http://docs.opencv.org/3.0-beta/doc/tutorials/calib3d/camera_calibration/camera_calibration.html

========================= =============================================================================================================================
Name                      Description
========================= =============================================================================================================================
Input                     Input images in one of the following form: - folder containing images - image sequence like "/path/to/seq.@.jpg" - video file
Pattern                   Type of pattern (camera calibration patterns) - **CHESSBOARD** - CIRCLES - ASYMMETRIC\ *CIRCLES - ASYMMETRIC*\ CCTAG
Size                      (Size of the Pattern) - Number of inner corners per one of board dimension like Width (**7**) Height (**5**) (0-10000)
Square Size               Size of the grid's square cells (0-100mm) (**1**)
Nb Distortion Coef        Number of distortion coefficient (0-5) (**3**)
Max Frames                Maximal number of frames to extract from the video file (0-5) (**0**)
Calib Grid Size           Define the number of cells per edge (0-50)
Max Calib Frames          Maximal number of frames to use to calibrate from the selected frames (0-1000)
Min Input Frames          Minimal number of frames to limit the refinement loop (0-100)
Max Total Average Error   Max Total Average Error (0-1)
Debug Rejected Img Folder Folder to export delete images during the refinement loop
Debug Selected Img Folder Folder to export debug images
Output                    Output filename for intrinsic [and extrinsic] parameters (default filename cameraCalibration.cal)
========================= =============================================================================================================================
