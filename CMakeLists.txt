# Should be compatible with unix and 
# windows using cygwin and crosscompiling using mingw
# also don't forget to edit config.cmake     

cmake_minimum_required(VERSION 3.15)
project(AFAP ) # Needs to be ontop

message(STATUS "Building the base modules")

add_subdirectory(Math_extra)
add_subdirectory(Omp_extra)

add_subdirectory(aCorrs-OTF)
add_subdirectory(FFTW_extra)
add_subdirectory(Multi_array)
add_subdirectory(Time_quadratures)
add_subdirectory(Histograms)

