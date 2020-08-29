cmake_minimum_required(VERSION 3.5)
cmake_policy(SET CMP0077 OLD)
project(latijns_json)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

add_library(latijns_json "inc/latijns/json.hpp" "src/json.cpp")
target_include_directories(latijns_json PUBLIC  "inc")
target_include_directories(latijns_json PRIVATE "src")
