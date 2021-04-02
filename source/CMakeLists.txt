cmake_minimum_required(VERSION 3.12)

# default language: C C++
project(LearnOpenGL)

set(DEPENDENCY_PATH C:\\Users\\syf\\Projects\\Dependencies)

add_executable(main main.cpp glad.c)

target_link_libraries(main PRIVATE 
                            ${DEPENDENCY_PATH}\\Libs\\glfw3.lib
                            opengl32.lib)
target_include_directories(main PRIVATE ${DEPENDENCY_PATH}\\Include)
