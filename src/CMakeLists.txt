file(GLOB_RECURSE LIB_SRC "*.cc")

set(LIB_INCLUDES "${PROJECT_SOURCE_DIR}/include/")
add_library(${LIB} OBJECT ${LIB_SRC})
target_include_directories(${LIB} PUBLIC ${LIB_INCLUDES})
target_link_libraries(${LIB} ${CONAN_LIBS})
target_compile_features(${LIB} PUBLIC cxx_std_20)