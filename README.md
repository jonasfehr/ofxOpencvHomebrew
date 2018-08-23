# ofxOpencvHomebrew
openFrameworks addon to to use openCV installed with homebrew on OSX


Introduction
------------
Instead of ofxOpenCV you can use this addon to add the necessary flags to your xcode file.

Installation
------------
1. Copy to your openFrameworks/addons folder or use <code>git clone</code>
2. Use the Project generator to create your project.
3. Check if the following lines are correctly added to your Xcode Project file

LINKER FLAGS 
to create your own list use following line in your terminal:
pkg-config --cflags --libs /usr/local/Cellar/opencv/3.4.2/lib/pkgconfig/opencv.pc

```sh
-I/usr/local/Cellar/opencv/3.4.2/include/opencv -I/usr/local/Cellar/opencv/3.4.2/include -L/usr/local/Cellar/opencv/3.4.2/lib -lopencv_stitching -lopencv_superres -lopencv_videostab -lopencv_aruco -lopencv_bgsegm -lopencv_bioinspired -lopencv_ccalib -lopencv_dnn_objdetect -lopencv_dpm -lopencv_face -lopencv_photo -lopencv_fuzzy -lopencv_hfs -lopencv_img_hash -lopencv_line_descriptor -lopencv_optflow -lopencv_reg -lopencv_rgbd -lopencv_saliency -lopencv_stereo -lopencv_structured_light -lopencv_phase_unwrapping -lopencv_surface_matching -lopencv_tracking -lopencv_datasets -lopencv_dnn -lopencv_plot -lopencv_xfeatures2d -lopencv_shape -lopencv_video -lopencv_ml -lopencv_ximgproc -lopencv_calib3d -lopencv_features2d -lopencv_highgui -lopencv_videoio -lopencv_flann -lopencv_xobjdetect -lopencv_imgcodecs -lopencv_objdetect -lopencv_xphoto -lopencv_imgproc -lopencv_core</code>
```

HEADER SEARCH PATH
```sh
/usr/local/Cellar/opencv/3.4.2/include</code>
```

LIBRARY SEARCH PATH (!!! THIS ONE NEEDS TO BE ADDED MANUALT)
```sh
/usr/local/Cellar/opencv/3.4.2/lib</code>
```
