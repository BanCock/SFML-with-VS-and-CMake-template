# SFML and ImGui with Visual Studio and CMake WSL2 template

I made this repository template to make my future work easier. 
This template serves as the basis for future projects using SFML and ImGui (unless I give it up, of course).

[Templates](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) are used to fork repositories without inheriting its Git history.

This template is based on [cmake-sfml-project](https://github.com/SFML/cmake-sfml-project) template, and there are likely elements that I have not yet understood or noticed because I have no experience, so criticism is welcome.

# Features

1. [ImGui](https://github.com/ocornut/imgui) and [ImGui-SFML](https://github.com/SFML/imgui-sfml) are included in the project, located in deps, files related to git were deleted due to the fact that they take up a lot of space.

2. [SFML](https://www.sfml-dev.org/index.php) is not stored in this project, so it is necessary that it be installed on the system. You can install it in your system using:
 ```
    sudo apt update
    sudo apt-get install libsfml-dev
 ```
3. Or you can configure the project so that sfml will be installed during build. Need to change a CMakeLists files. 
Open [this](deps/CMakeLists.txt) and [this](deps/sfml/CMakeLists.txt) files and follow commented instructions.

4. For more instructions and information take a look at the sources:
 - [ImGui-SFML](https://github.com/SFML/imgui-sfml) - сontains a useful information about imgui-sfml projects, I largely followed the guides from there.
 - [Crossplatform development using VS and WSL2](https://learn.microsoft.com/en-us/cpp/build/walkthrough-build-debug-wsl2?view=msvc-170) - I want to use Visual Studio to make projects in WSL2, so this article helped me a lot.
 - [ImGui wiki](https://github.com/ocornut/imgui/wiki) - documentation for detailed information about the imgui's capabilities.
 - [Template that i took](https://github.com/SFML/cmake-sfml-project) - information about buildin sfml projects with different configurations and for different IDEs.
 - [CMake documentation](https://cmake.org/cmake/help/latest/) - this is my first CMake experience, so I often came here with questions about CMake.
