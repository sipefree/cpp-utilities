# eteran / cpp-utilities / container / test / FlatMapTest
cmake_minimum_required(VERSION 3.5)


project("${PROJECT_NAME}-test-FlatMap" CXX)
add_executable("${PROJECT_NAME}" "")


target_sources(
	"${PROJECT_NAME}"
	PRIVATE
		"${CMAKE_CURRENT_LIST_DIR}/FlatMap.cpp"
)


target_link_libraries(
	"${PROJECT_NAME}"
	PRIVATE
		eteran::cpp-utilities::container
		eteran::cpp-utilities::defaults
)


add_test("${PROJECT_NAME}" "${PROJECT_NAME}")

