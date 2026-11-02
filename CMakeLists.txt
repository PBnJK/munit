cmake_minimum_required(VERSION 3.28)
project(
	munit
	VERSION 0.2.0
	LANGUAGES C
)

add_library(${PROJECT_NAME} "munit.c")

target_include_directories(${PROJECT_NAME} PRIVATE "${PROJECT_SOURCE_DIR}")
target_compile_features(${PROJECT_NAME} PRIVATE "c_std_99")
target_compile_options(${PROJECT_NAME} PRIVATE "-Wall" "-Wextra" "-pedantic")
