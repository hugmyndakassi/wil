
add_executable(witest)

target_precompile_headers(witest PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/../pch.h)

target_sources(witest PRIVATE
    ${COMMON_SOURCES}
    ${CMAKE_CURRENT_SOURCE_DIR}/../NetworkTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../RegistryTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../StlTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../TokenHelpersTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../UniqueWinRTEventTokenTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../WatcherTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../WinRTTests.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/../WinVerifyTrustTest.cpp
    )
