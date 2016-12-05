set (SRC_LIST
 id.cc
 id.h
)

add_library(snowflake4cxx STATIC ${SRC_LIST})
target_link_libraries(snowflake4cxx)

set (ID_TEST_LIST
  id_test.cc
  )

add_executable (id_test ${ID_TEST_LIST})
target_link_libraries (id_test snowflake4cxx)


