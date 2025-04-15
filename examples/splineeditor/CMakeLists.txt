file(GLOB_RECURSE splineeditor_SRCS *.h *.cpp)

add_qwt_example(splineeditor "${splineeditor_SRCS}")  