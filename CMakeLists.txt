cmake_minimum_required(VERSION 3.15)
project(MiniDB CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if (CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
    add_compile_options(-Wall -Wextra)
endif()

find_package(Threads REQUIRED)

add_executable(minidb src/main.cpp)
target_link_libraries(minidb PRIVATE Threads::Threads)
