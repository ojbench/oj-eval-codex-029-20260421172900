cmake_minimum_required(VERSION 3.10)
project(problem_029_malloc C)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

add_executable(code src/main.c)

if (CMAKE_C_COMPILER_ID MATCHES "GNU|Clang")
  target_compile_options(code PRIVATE -O2 -Wall -Wextra -Werror -Wno-unused-parameter)
endif()

