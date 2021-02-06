find_package(glfw3 3.3 REQUIRED)
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(triangle triangle.cc)
add_executable(square square.cc)

target_link_libraries(triangle glfw)
target_link_libraries(triangle OpenGL::GL)
target_link_libraries(triangle GLEW::GLEW)
target_link_libraries(square glfw)
target_link_libraries(square OpenGL::GL)
target_link_libraries(square GLEW::GLEW)
