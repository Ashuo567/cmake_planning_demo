project(pnc_map)  # 只需要生成动态库，因为没有调用其他库，所以不需要再链接其他库

# 生成动态库
add_library(${PROJECT_NAME}
SHARED
pnc_map.cpp
)
