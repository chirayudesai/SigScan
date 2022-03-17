cmake_minimum_required(VERSION 3.10)
project(SigScan)

set(SRCS src/main.cpp src/SigScan.cpp)
set(LIBS Boost::program_options)

set(CMAKE_CXX_STANDARD 17)

find_package(Boost COMPONENTS program_options REQUIRED)

add_executable(${PROJECT_NAME} ${SRCS})
target_link_libraries(${PROJECT_NAME} ${LIBS})
