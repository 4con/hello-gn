Try for google gn build on Windows. 

Use open source chromium project files, the chromium project license see LICENSE file.

the build\ and tools\ folder contain files from chromium project. (Some files may not be used.)

1. Open cmd and cd to current directory. Find and clone gyp repo to tools/gyp.

2. run `env.bat` to setup VS compile environment.

3. Generate ninja.build with gn.

`gn gen out/Default`

For see what args supported, using `gn args --list out/Default`

4. Build with ninja

`ninja -C out/Default`