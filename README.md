### 同步安卓源码 ###

```bash

# 清华源节点（然而并不是）

$ repo init -u https://android.googlesource.com/platform/manifest -b android-10.0.0_r41

# 同步源码

$ repo sync
```
### 下载device tree ###

```txt
/device/brand/device
/kernel/brand/device
/vendor/brand/device
如果使用私人开发者的device tree可能还需要更多的文件
```

### 修改device文件夹下部分文件 ###

### 编译 ###

```bash

# 初始化编译环境
$ source build/envsetup.sh

# 选择目标设备
$ lunch

# 编译
$ make -j8
```

### 已有源码切换分支 ###

```bash

$ repo init -b android-10.0.0_r41

```
