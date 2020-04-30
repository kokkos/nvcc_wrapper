# Kokkos NVCC Wrapper

This wraps an nvcc, allowing it to be treated as a real C++ compiler with all the usual flags.
Simple run `cmake` as usual to configure the compiler. The only two flags that need to be set are:
````
-DCMAKE_CXX_COMPILER=
-DCMAKE_CUDA_COMPILER=
````
so that the wrapper knows which underlying `nvcc` and which underlying `g++` to use.
This is configured as both a CXX and CUDA project with CMake, which means a valid
CUDA installation must be available.

