cmake_minimum_required(VERSION 2.8)
project( stitching )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( stitching stitching.cpp )
target_link_libraries( stitching ${OpenCV_LIBS} )