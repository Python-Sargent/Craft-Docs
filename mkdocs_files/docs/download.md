## Download

See below to run from source.

## Install Dependencies

It is best to update your OS and it's packages before adding new ones.

Linux (Debain, Raspbian, Ubuntu):
```sh
sudo apt-get update
```

Linux (ARCH-Linux):
```
pacman -Syu
```

MacOS X:
```
sudo softwareupdate -i -a -R
```

Windows

Check for updates.

---

### Mac OS X

Download and install [CMake](http://www.cmake.org/cmake/resources/software.html)
if you don't already have it. You may use [Homebrew](http://brew.sh) to simplify
the installation:

```zsh
brew install cmake
```

### Linux (Ubuntu)

```sh
sudo apt-get install cmake libglew-dev xorg-dev libcurl4-openssl-dev
sudo apt-get build-dep glfw
```

### Linux (ARCH-Linux)

```sh
pacman -S cmake libglew-dev xorg-dev libcurl4-openssl-dev
pacman -S build-dep glfw
```

### Windows

#### Using MinGW
Download and install [CMake](http://www.cmake.org/cmake/resources/software.html)
and [MinGW](https://www.mingw-w64.org/downloads/). Add `C:\MinGW\bin` to your `PATH`.

#### Using MSYS2
Download and Install [MSYS2](https://www.msys2.org/) and [CMake](http://www.cmake.org/cmake/resources/software.html)
run MSYS2 terminal and use `pacman` to install `mingw-w64-x86_64-cmake` and `mingw-w64-x86_64-make`. Run the following:

```shell
pacman -S mingw-w64-x86_64-cmake
pacman -S mingw-w64-x86_64-make
```

#### Get cURL

Download and install [cURL](http://curl.haxx.se/download.html) so that
CURL/lib and CURL/include are in your Program Files directory.

Use the following commands in place of the ones described in the next section.

```shell
cmake -G "MinGW Makefiles"
mingw32-make
```

---

## Compile and Run

Once you have the dependencies (see above), run the following commands in your
terminal.

```shell
git clone https://github.com/Python-Sargent/Craft.git
cd Craft
cmake .
make
./craft
```

This will clone the repo, move your working directory to the repo directory and use `cmake` to get the build ready to compile using `make`.
Then the `craft` binary is run using `./craft`. You can now enjoy Craft.

---