cmake_minimum_required(VERSION 3.17)

project(qwt)

set(CMAKE_AUTOMOC ON)
set(CMAKE_CXX_STANDARD 17)

option(QWT_DLL "build the static/shared libraries." ON)
option(QWT_PLOT "enable all classes, that are needed to use the QwtPlot widget." ON)
option(QWT_POLAR "enable all classes, that are needed to use the QwtPolar classes. It can't be enabled without also enabling QwtPlot." ON)
option(QWT_WIDGETS "enable all classes, that are needed to use the all other widgets (sliders, dials, ...), beside QwtPlot." ON)
option(QWT_SVG "If you want to display svg images on the plot canvas, or export a plot to a SVG document." ON)
option(QWT_OPENGL "If you want to use a OpenGL plot canvas" ON)
option(QWT_EXAMPLES "If you want to use a OpenGL plot canvas" OFF)

set(QWT_ROOT ${CMAKE_CURRENT_SOURCE_DIR})
set(QWT_CLASS_INCLUDE_PATH ${QWT_ROOT}/classincludes)

find_package(Qt6 COMPONENTS Core Gui Xml Widgets PrintSupport Concurrent REQUIRED)

if (QWT_SVG)
    find_package(Qt6 COMPONENTS Svg REQUIRED)
else()
    add_compile_definitions(QWT_NO_SVG)
endif()

if (QWT_OPENGL)
    find_package(Qt6 COMPONENTS OpenGLWidgets REQUIRED)
else()
    add_compile_definitions(QWT_NO_OPENGL)
endif()

if (MSVC)
    add_compile_options("$<$<C_COMPILER_ID:MSVC>:/utf-8>")
    add_compile_options("$<$<CXX_COMPILER_ID:MSVC>:/utf-8>")
endif()

add_subdirectory(src)
if (QWT_EXAMPLES)
    add_subdirectory(examples)
endif()
