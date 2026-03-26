# 2.5D

## Compilation tips (for project)

specifying the path explicitly
- `g++ main.cpp -o prog -L./SDL/mybuild/libSDL3.so.0.5.0 -lSDL3`

alternative
install the library by
- `sudo make install`
in the build directory of sdl3
afterwards it can be compiled using
- `g++ main.cpp -o prog -lSDL3`

Optional:
-  `pkg-config sdl3`
-  `pkg-config --libs --cflags sdl3`

findout all the header files references by program
`g++ -H main.cpp`

## Compilation of SDL from git repository

- `git clone git@github.com-work:libsdl-org/SDL.git`
- `cd SDL`
- `mkdir mybuild && cd mybuild`
- `cmake ..`
- `make -j 4`
