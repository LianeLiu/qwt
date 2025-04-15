file(GLOB_RECURSE dials_SRCS *.h *.cpp)

add_qwt_example(dials "${dials_SRCS}")  