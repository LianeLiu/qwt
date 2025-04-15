file(GLOB_RECURSE animation_SRCS *.h *.cpp)

add_qwt_example(animation "${animation_SRCS}")  