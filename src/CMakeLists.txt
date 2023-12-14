#子目录下的源文件，取名为TEST_SRC,让父级目录可见
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} BASE_P_SRC)
set(BASE_P_SRC ${BASE_P_SRC} PARENT_SCOPE)