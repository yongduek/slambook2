project(stereoVision)

find_package(Pangolin REQUIRED)
find_package(OpenCV REQUIRED)
message("OpenCV_DIRS: ${OpenCV_DIRS}")
message("OpenCV_LIBS: ${OpenCV_LIBS}")

add_executable(stereoVision stereoVision.cpp)
target_link_libraries(stereoVision ${OpenCV_LIBS} ${Pangolin_LIBRARIES})