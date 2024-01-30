message(STATUS "linking SFML...")

# No need to build audio and network modules
set(SFML_BUILD_AUDIO FALSE)
set(SFML_BUILD_NETWORK FALSE)

# Uncomment it if you want sfml 
# to install in your project during building time
# and go to the deps/CMakeLists.txt

#FetchContent_MakeAvailable(sfml)