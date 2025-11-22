cmake_minimum_required(VERSION 3.10)
project(planning
	VERSION 0.0.1 
	DESCRIPTION "a demo of cmake planning" 
	HOMEPAGE_URL "git clone https://github.com/stewie-2025/cmake_planing_demo"
) 

set(CMAKE_CXX_STANDARD 11)

#变量和目录设置
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin) 
set(Process_Dir ${CMAKE_SOURCE_DIR}/src/process)
set(PNC_Map_Dir ${CMAKE_SOURCE_DIR}/src/pnc_map)


#添加子目录--只要src目录有CMakeLists它就会找到
add_subdirectory(src)
