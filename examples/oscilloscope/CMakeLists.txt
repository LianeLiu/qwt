file(GLOB_RECURSE oscilloscope_SRCS *.h *.cpp)

add_qwt_example(oscilloscope "${oscilloscope_SRCS}")  