cmake_minimum_required(VERSION 3.27.1)

include(${WORKSPACE}/sdk/cmake/common.cmake)

sdk_project(PIC64GX_Setup_Test_270826)

target_sources(${PROJECT_NAME} PUBLIC
	${CMAKE_CURRENT_SOURCE_DIR}/src/application/hart0/e51.c
	${CMAKE_CURRENT_SOURCE_DIR}/src/application/hart1/u54_1.c
	${CMAKE_CURRENT_SOURCE_DIR}/src/application/hart2/u54_2.c
	${CMAKE_CURRENT_SOURCE_DIR}/src/application/hart3/u54_3.c
	${CMAKE_CURRENT_SOURCE_DIR}/src/application/hart4/u54_4.c

)

target_include_directories(${PROJECT_NAME} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/src/application/
)