add_executable(main main.cpp)

target_link_libraries(main glfw glad)

if (APPLE)
    target_link_libraries(main "-framework OpenGL")
elseif (WIN32)
    target_link_libraries(main opengl32)
else()
    target_link_libraries(main GL)
endif()