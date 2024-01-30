include(FetchContent)

#FetchContent_Declare(
#  sfml
#  GIT_REPOSITORY "https://github.com/SFML/SFML"
#  GIT_TAG 69ea0cd863aed1d4092b970b676924a716ff718b # 2.6.1
#)
find_package(SFML REQUIRED graphics)

add_subdirectory(sfml)

FetchContent_Declare(
  imgui
  GIT_REPOSITORY https://github.com/ocornut/imgui
  GIT_TAG d6cb3c923d28dcebb2d8d9605ccc7229ccef19eb # 1.90.1
)
FetchContent_MakeAvailable(imgui)

FetchContent_Declare(
  imgui-sfml
  GIT_REPOSITORY https://github.com/SFML/imgui-sfml
  GIT_TAG de565ac8f2b795dedc0307b60830cb006afd2ecd
)

set(IMGUI_DIR ${CMAKE_SOURCE_DIR}/deps/imgui)
set(IMGUI_SFML_FIND_SFML OFF)
set(IMGUI_SFML_IMGUI_DEMO ON)

FetchContent_MakeAvailable(imgui-sfml)
