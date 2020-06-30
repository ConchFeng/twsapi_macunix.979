cmake_minimum_required(VERSION 3.12)
project(ib-api-test)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "-pthread -Wall")

add_subdirectory(IBJts/source/cppclient/client)
add_subdirectory(IBJts/samples/Cpp/TestCppClient)
