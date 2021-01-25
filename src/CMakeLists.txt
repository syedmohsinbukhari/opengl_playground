find_package(glfw3 3.3 REQUIRED)
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(opengl_window opengl_window.cc)

target_link_libraries(opengl_window glfw)
target_link_libraries(opengl_window OpenGL::GL)
target_link_libraries(opengl_window GLEW::GLEW)
