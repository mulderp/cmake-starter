set(APP_SOURCES main.cpp)
set(LIB_SOURCES mylib/world.cpp)

# creates ./build/bin/runner
add_executable(${PROJECT_NAME} ${APP_SOURCES})

# shared library
set(LIBRARY_NAME World)
add_library(${LIBRARY_NAME} SHARED ${LIB_SOURCES})
target_link_libraries(${PROJECT_NAME} ${LIBRARY_NAME})
