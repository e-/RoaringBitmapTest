CMAKE_MINIMUM_REQUIRED(VERSION 3.1)
project(ROARING_BITMAP_TEST)

if (NOT CMAKE_BUILD_TYPE)
  message(STATUS "No build type selected, default to Release")
  set(CMAKE_BUILD_TYPE Release CACHE STRING "Choose the type of build." FORCE)
endif()

set(ROARING_BITMAP_TEST_LIB_NAME ROARING_BITMAP_TEST)
set(ROARING_BITMAP_TEST_VERSION 0.0.1)

include_directories(include)

add_subdirectory(src)

message( STATUS "CMAKE_SYSTEM_PROCESSOR: " ${CMAKE_SYSTEM_PROCESSOR})
message( STATUS "CMAKE_BUILD_TYPE: " ${CMAKE_BUILD_TYPE} )
message( STATUS "CMAKE_CXX_COMPILER: " ${CMAKE_CXX_COMPILER} ) # important to know which compiler is used
message( STATUS "CMAKE_CXX_FLAGS: " ${CMAKE_CXX_FLAGS} ) # important to know the flags
message( STATUS "CMAKE_CXX_FLAGS_DEBUG: " ${CMAKE_CXX_FLAGS_DEBUG} )
message( STATUS "CMAKE_CXX_FLAGS_RELEASE: " ${CMAKE_CXX_FLAGS_RELEASE} )