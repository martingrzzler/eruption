set(APP_SRC main.cc)

add_executable(${MAIN} ${APP_SRC})
target_link_libraries(${MAIN} PUBLIC ${LIB})
target_include_directories(${MAIN} PUBLIC ${PROJECT_BINARY_DIR})