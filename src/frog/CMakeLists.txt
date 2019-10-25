add_library(frog SHARED ./src/frog.cpp)
set_target_properties(frog PROPERTIES CXX_STANDARD 14 CXX_STANDARD_REQUIRED YES CXX_EXTENSIONS NO)
target_include_directories(frog PUBLIC ./include)
