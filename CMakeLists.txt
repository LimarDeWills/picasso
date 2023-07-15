# cmake_minimum_required(VERSION 3.13)

# project(picasso)

# find_package(OpenGL REQUIRED)

# set(SRC_FILES
#     src/main.cpp
# )
# # add_subdirectory(vendor/glad)

# # add_subdirectory(vendor/glfw)

# add_executable(picasso ${SRC_FILES})

# include_directories(
#     include
#     vendor/glad/include
#     ${OPENGL_INCLUDE_DIRS}
# )
# # include_directories(   ${GLUT_INCLUDE_DIRS} )

# # target_link_libraries(testas  ${GLUT_LIBRARY} )

# target_link_libraries(picasso glad glfw ${OPENGL_LIBRARIES})

cmake_minimum_required(VERSION 3.13)

set(project_name picasso)
project(${project_name})

set(PICASSO_SRC
    src/main.cpp
)

add_subdirectory(vendor/glfw)
add_subdirectory(vendor/glad)

add_executable(${project_name} ${PICASSO_SRC})

include_directories(
    include
    vendor/glad/include
    vendor/glfw/include
)
target_link_libraries(${project_name} glad glfw)