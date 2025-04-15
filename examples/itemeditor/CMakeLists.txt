file(GLOB_RECURSE itemeditor_SRCS *.h *.cpp)

add_qwt_example(itemeditor "${itemeditor_SRCS}")  