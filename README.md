Sample cmake 3.15 C++14 project built in android 6.0 using clang 8.0 in termux (0.75 from fdroid).

It is a simple executable which is linked to a simple shared library.

To build, first clean the build dir:
cd ./build
rm -rf *

Then built from the build dir:
cmake ../src

Then the executable ./app/main can be run, but it needs the shared library built during previous step which should be findable(?) in the usual library path:
LD_LIBRARY_PATH="${LD_LIBRARY_PATH}":$(cd ./frog && pwd) ./app/main
