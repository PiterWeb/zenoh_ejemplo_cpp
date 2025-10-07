Antes de ejecutar hay que instalar zenoh, [zenoh-c](https://github.com/eclipse-zenoh/zenoh-c) y después [zenoh-cpp](https://github.com/eclipse-zenoh/zenoh-cpp).

## Prebuild

1. Instalar rust
2. git clone https://github.com/eclipse-zenoh/zenoh-c.git
3. mkdir -p build && cd build 
4. cmake ../zenoh-c
5. cmake --build . --config Release
6. cmake --build . --target install
7. git clone https://github.com/eclipse-zenoh/zenoh-cpp.git
8. mkdir build && cd build
9. cmake .. -DCMAKE_INSTALL_PREFIX=~/.local

## Build (en directorio raiz del proyecto)

1. mkdir build
2. chmod +x build.sh
3. ./build.sh
