add_executable(CMakeSFMLProject main.cpp)
target_link_libraries(CMakeSFMLProject PRIVATE sfml-graphics)
target_link_libraries(CMakeSFMLProject PRIVATE ImGui-SFML::ImGui-SFML)
