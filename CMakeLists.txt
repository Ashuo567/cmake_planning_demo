cmake_minimum_required(VERSION 3.29.0)
project(planning
    VERSION 0.0.1
    DESCRIPTION "a demo of cmake planning"
    HOMEPAGE_URL "https://github.com/Ashuo567/cmake_planning_demo"
    LANGUAGES CXX
)
set(CMAKE_CXX_STANDARD 17)

# 变量设置(动态库及可执行文件的输出目录)  (该变量会传递给子目录用)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(Process_Dir ${CMAKE_SOURCE_DIR}/src/process)
set(PNC_Map_Dir ${CMAKE_SOURCE_DIR}/src/pnc_map)
set(Show_Result_Dir ${CMAKE_SOURCE_DIR}/src/show_result)


# 添加子目录
add_subdirectory(src)