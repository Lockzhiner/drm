# 安装modetest

## 版本

|文档版本|修改人|修改内容简介|
|-|-|-|
|0_0_0|郑必城|初步完成文档编写|


## 简介

modetest 是由 libdrm 提供的测试程序，可以查询显示设备的特性，进行基本的显示测试，以及设置显示的模式。

## 编译过程

```Bash
sudo apt install meson
sudo apt install cmake
sudo apt-get install -y libatomic-ops-dev
sudo apt-get install libpciaccess-dev
git clone https://gitlab.freedesktop.org/mesa/drm
git checkout libdrm-2.4.95
meson build
sudo ninja -C build install
cd build/tests/modetest/
sudo cp ./modetest /bin
```

## 使用教程

```Bash
# 查看使用方式
modetest -h
```