cmake_minimum_required(VERSION 3.28)

project(MyTemplate)

# Define exectuable target
add_executable(MyApp)

# Set C++ standard
target_compile_features(MyApp PUBLIC cxx_std_17)

# Set compiler options
target_compile_options(MyApp PRIVATE -Wall -Werror)

# Set sources
target_sources(MyApp
  PRIVATE
    main.cpp
)

# Link internal libraries
target_link_libraries(MyApp PRIVATE MyLibrary)


