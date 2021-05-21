cmake_minimum_required(VERSION 3.10)
project(solr LANGUAGES CXX CUDA)

#######################################
# Core Library
#######################################

include_directories("solr/")
add_library(
    solr    
)

set_property(TARGET solr PROPERTY CUDA_SEPARABLE_COMPILATION ON)

target_include_directories(
    solr PUBLIC
    "G:/NVIDIA GPU Computing Toolkit/CUDA/v11.3/include/common/inc"   
)

