file(GLOB_RECURSE spectrogram_SRCS *.h *.cpp)

add_qwt_example(spectrogram "${spectrogram_SRCS}")  