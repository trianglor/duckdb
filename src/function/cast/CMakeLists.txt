add_library_unity(
  duckdb_func_cast
  OBJECT
  blob_cast.cpp
  cast_function_set.cpp
  decimal_cast.cpp
  default_casts.cpp
  enum_casts.cpp
  list_casts.cpp
  map_cast.cpp
  numeric_casts.cpp
  pointer_cast.cpp
  string_cast.cpp
  struct_cast.cpp
  time_casts.cpp
  uuid_casts.cpp)

set(ALL_OBJECT_FILES
    ${ALL_OBJECT_FILES} $<TARGET_OBJECTS:duckdb_func_cast>
    PARENT_SCOPE)
