file(GLOB_RECURSE sysinfo_SRCS *.h *.cpp)

add_qwt_example(sysinfo "${sysinfo_SRCS}")  