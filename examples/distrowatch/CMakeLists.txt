file(GLOB_RECURSE distrowatch_SRCS *.h *.cpp)

add_qwt_example(distrowatch "${distrowatch_SRCS}")  