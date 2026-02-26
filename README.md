luv
===
MSYS2로 빌드된 MPV에 통합하는 방법

1. cmake
```
cmake .. -G "Ninja" \
  -DCMAKE_C_COMPILER=clang \
  -DBUILD_MODULE=ON \
  -DBUILD_SHARED_LIBS=OFF \
  -DWITH_SHARED_LIBUV=OFF \
  -DLUA_BUILD_TYPE=System
```
2. build by ninja
```
ninja
```
