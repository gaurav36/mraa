add_executable (AioA0 AioA0.cpp)
add_executable (blink-io-cpp Blink-IO.cpp)
add_executable (Pwm3-cycle Pwm3-cycle.cpp)
add_executable (I2c-compass I2c-compass.cpp)
add_executable (Spi-pot Spi-pot.cpp)

include_directories(${PROJECT_SOURCE_DIR}/api)

target_link_libraries (AioA0 mraa stdc++)
target_link_libraries (blink-io-cpp mraa stdc++)
target_link_libraries (Pwm3-cycle mraa stdc++)
target_link_libraries (I2c-compass mraa stdc++ m)
target_link_libraries (Spi-pot mraa stdc++)
