安装 meson



sudo apt install python3-pip
pip3 install meson==0.63



安装 aarch64-linux-gnu-pkg-config  sudo apt install pkg-config-aarch64-linux-gnu

$ meson --prefix=/home/zhangsz/rtt/glib/libs --cross-file cross_aarch64_musl.txt builddir

meson --prefix=/home/rtt/smart/libs/glib_libs --cross-file cross_aarch64_musl.txt builddir
ninja -C builddir
ninja -C builddir install


## 编译静态库与动态库

meson --prefix=/home/zhangsz/rtt/glib/libs -Ddefault_library=both --cross-file cross_aarch64_musl.txt builddir

