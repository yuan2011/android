# BootImgTool
A Tool for unpack/pack android boot.img

Combined these two projects:

https://github.com/pbatard/bootimg-tools

https://github.com/sophiehuiberts/Bootimg-scripts

Add some usefull script for convenience

# Usage

1. compile
```
./build.sh
```

2. unpack
```
./bin/unpack-bootimg.sh path/of/boot.img
```

 boot.img
 boot.img-kernel.gz //替换kernel时，覆盖此文件
 boot.img-ramdisk //进入此目录修改配置
 boot.img-ramdisk.cpio.gz


3. repack 暂未处理cmdline
```
bin/repack-bootimg.sh kernel ramdisk-dir out-file
```
如：
bin/repack-bootimg.sh tmp/boot.img-kernel.gz tmp/boot.img-ramdisk boot.img
