qt5_wrap_cpp(hello-world_SRC ${HW_HEADER_DIR}/MainWindow.h)
qt5_wrap_ui(hello-world_UI ${HW_GUI_DIR}/MainWindow.ui)

set(SOURCE_FILES MainWindow.cpp
                 main.cpp)

add_executable(hello-world ${SOURCE_FILES} ${hello-world_UI} ${hello-world_SRC})
target_link_libraries(hello-world Qt5::Widgets)
