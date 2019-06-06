cmake_minimum_required(VERSION 3.11)
project(HelloWorld)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_EXTENSIONS OFF)


set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -DWIN_TEST -I../source -I../cpputest/include -Wall -Wextra -Wno-long-long -pedantic")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -DWIN_TEST -I../source -I../cpputest/include -Wall -Wextra -Wno-long-long -pedantic")

add_executable(HelloWorld.exe
  ./main.c
)

