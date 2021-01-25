find_package(glfw3 3.3 REQUIRED)
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(triangle triangle.cc)

target_link_libraries(triangle glfw)
target_link_libraries(triangle OpenGL::GL)
target_link_libraries(triangle GLEW::GLEW)
