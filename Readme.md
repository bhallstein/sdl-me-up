# SDL-Me-Up

[The SDL library](https://github.com/libsdl-org/SDL), prepped for use as a submodule-style dependency.

**Current release:** release-2.0.22


### Contents

- `/include` — SDL's include path
- `/mac/libSDL2.a` — SDL compiled as a static library for mac (x64 and arm)


### Mac usage instructions

- Add `sdl-me-up/include` as a header search path
- Add libSDL2.a as a static library or framework
- Add other frameworks that are required by SDL
- Command line example:

```bash
clang++ -std=c++14 my-game.cpp \
  -I sdl-me-up/include \
  -L lib -l SDL2 \
  -framework AudioToolbox \
  -framework Carbon \
  -framework Cocoa \
  -framework CoreAudio \
  -framework CoreGraphics \
  -framework CoreVideo \
  -framework ForceFeedback \
  -framework IOKit \
  -framework Metal \
  -o my-game
```
