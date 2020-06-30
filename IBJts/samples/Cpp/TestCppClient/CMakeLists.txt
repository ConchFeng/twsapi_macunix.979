set(PROJECT_NAME TestCppClient)

file(GLOB TestCppClient-header "*.h")
file(GLOB TestCppClient-source "*.cpp")

include_directories(${PROJECT_SOURCE_DIR}/IBJts/source/cppclient/)
include_directories(${PROJECT_SOURCE_DIR}/IBJts/source/cppclient/client)

add_executable(${PROJECT_NAME} ${TestCppClient-header} ${TestCppClient-source})

target_link_libraries(${PROJECT_NAME} client-lib)
