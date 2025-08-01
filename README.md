# FluentSTL

FluentSTL is a C++ library that implements optimized STL-like
containers. It was designed to be used with C++20 and later, and it
is the main library used in the Fluent Programming Language.

## Installing

Use CMake:
```cmake
include(FetchContent)

FetchContent_Declare(
        fluent_stl
        GIT_REPOSITORY https://github.com/fluent-lang/STL.git
        GIT_TAG        master
)

FetchContent_MakeAvailable(fluent_stl)
target_link_libraries(Fluent PRIVATE fluent::stl)
```

## License

FluentSTL is licensed under the GNU General Public License v3.0
(GPL-3.0). You can find the full license text in the `LICENSE`
file in the root directory of this repository.
