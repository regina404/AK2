cmake_minimum_required(VERSION 2.8)	 # Проверка версии CMake.
										

project(hello_world)			

add_library(
	info 
	STATIC 
	info.cpp
)	# Создание статической библиотеки с именем info

add_executable(
	main 
	main.cpp
)	# Создает исполняемый файл с именем main

target_link_libraries(main info)		
