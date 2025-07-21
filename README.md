# freeseprite


# Windows (https://www.youtube.com/watch?v=82TIDyKjxuE)

call "C:\Program Files\Microsoft Visual Studio\2022\Community\Common7\Tools\VsDevCmd.bat" -arch=x64

cd C:/aseprite/build

cmake -DCMAKE_BUILD_TYPE=RelWithDebInfo -DLAF_BACKEND=skia -DSKIA_DIR=C:\deps\skia -DSKIA_LIBRARY_DIR=C:\deps\skia\out\Release-x64 -DSKIA_LIBRARY=C:\deps\skia\out\Release-x64\skia.lib -G Ninja ..

ninja aseprite

and second: To fix error with .exe
ninja aseprite

and after that go to "C:\aseprite\build\bin"

copy 'data' and 'aseprite.exe' to clean folder when you want
