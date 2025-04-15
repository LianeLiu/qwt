file(GLOB_RECURSE refreshtest_SRCS *.h *.cpp)

add_qwt_example(refreshtest "${refreshtest_SRCS}")  