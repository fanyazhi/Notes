# Using SFML with CMake on Mac

Install SDL2 with homebrew:

```
$ brew install sfml
```

Add to `CMakeLists.txt` after `add_executable()`:

```
set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake_modules")
find_package(SFML REQUIRED system window graphics network audio)
if (SFML_FOUND)
    include_directories(${SFML_INCLUDE_DIR})
    target_link_libraries(SFMLDemo ${SFML_LIBRARIES})
endif()
```
Finally `#include <SFML/Graphics.hpp>`

---
More on [Creating an SFML roject](http://www.gamefromscratch.com/post/2015/06/02/Creating-an-SFML-project-on-Mac-OS-using-CLion-and-CMake.aspx).