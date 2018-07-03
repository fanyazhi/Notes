# Using SDL2 with CMake on Mac

Install SDL2 with homebrew:

```
$ brew install sdl2
```

Add to `CMakeLists.txt`:

```
find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})
```

Add to `CMakeLists.txt` after `add_executable()`:

```
target_link_libraries(project_name ${SDL2_LIBRARIES})
```
Finally `#include "SDL.h"`

---
More on [Using SDL2 with CMake](https://trenki2.github.io/blog/2017/06/02/using-sdl2-with-cmake/).