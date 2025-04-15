file(GLOB_RECURSE stockchart_SRCS *.h *.cpp)

add_qwt_example(stockchart "${stockchart_SRCS}")  