cmake_minimum_required(VERSION 3.10)

project(ObjectDetection)

find_package(OpenCV REQUIRED)

add_executable(${PROJECT_NAME} src/main.cpp)
add_executable(image_show src/image.cpp)

target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
target_link_libraries(image_show ${OpenCV_LIBS})