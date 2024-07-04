project(process)

# 生成动态库
add_library(${PROJECT_NAME}
SHARED
process.cpp
)

# 包含头文件
target_include_directories(${PROJECT_NAME}
PUBLIC
${PNC_Map_Dir}
)

# 链接到动态库（即pnc_map）
target_link_libraries(${PROJECT_NAME}
PUBLIC
pnc_map
)
