cmake_minimum_required(VERSION 2.4)
project(CameraCalibration)

find_package( OpenCV REQUIRED )

include_directories( include ${OpenCV_INCLUDE_DIRS} )


set(SOURCE_FILES lab_homography_donald_skeleton.cpp)
add_executable(CV_donald_annotated_points ${SOURCE_FILES})

target_link_libraries( CV_donald_annotated_points ${OpenCV_LIBS} )
