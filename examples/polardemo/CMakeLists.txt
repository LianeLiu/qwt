file(GLOB_RECURSE polardemo_SRCS *.h *.cpp)

add_qwt_example(polardemo "${polardemo_SRCS}")  