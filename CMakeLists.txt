cmake_minimum_required(VERSION 3.28.0)
project(Test VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

#包含头文件
include_directories(include)

#工程目录下的原文件,命名为ROOT_SOURCE
aux_source_directory(. ROOT_SOURCE)

#指定一个子目录src,制定了src，cmake才回去src中找CMakeList
add_subdirectory(src)

#添加可执行文件，生成一个目标文件，取名为Test
add_executable(Test ${ROOT_SOURCE} ${BASE_P_SRC})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
