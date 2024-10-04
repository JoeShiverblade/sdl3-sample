## SDL3 App From Source Minimal Example
This is a minimal example for building and using SDL3 from source 
using C++ and CMake. It also demonstrates setting up things like macOS/iOS
bundles.
See [src/main.cpp](src/main.cpp) for the code. 

### Building And Running
Are you a complete beginner? If so, read [this](https://github.com/Ravbug/sdl3-sample/wiki/Setting-up-your-computer)!
Otherwise, install CMake and your favorite compiler, and follow the commands below:
```sh
# You need to clone with submodules, otherwise SDL will not download.
git clone https://github.com/Ravbug/sdl3-sample --depth=1 --recurse-submodules
cd sdl3-sample
cmake -S . -B build
```
You can also use an init script inside [`config/`](config/). Then open the IDE project inside `build/` 
(If you had CMake generate one) and run!

## Supported Platforms
I have tested the following:
- macOS
- iOS
- tvOS
- visionOS
- Windows
- Linux
- Web browsers (via Emscripten)*
- Android*

*See further instructions in [`config/`](config/)

Note: UWP support was [removed from SDL3](https://github.com/libsdl-org/SDL/pull/10731) during its development. For historical reasons, you can a working UWP sample via this commit: [df270da](https://github.com/Ravbug/sdl3-sample/tree/df270daa8d6d48426e128e50c73357dfdf89afbf)

## Updating SDL
Just update the submodule:
```sh
cd SDL
git pull
```
You don't need to use a submodule, you can also copy the source in directly. This
repository uses a submodule to keep its size to a minimum. Note that as of writing, SDL3 is
in development, so expect APIs to change. 


## Reporting issues
Is something not working? Create an Issue or send a Pull Request on this repository!
