file(GLOB_RECURSE polarspectrogram_SRCS *.h *.cpp)

add_qwt_example(polarspectrogram "${polarspectrogram_SRCS}")  