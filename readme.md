## install bochs
```
./configure --prefix=~/bochs --enable-debugger --enble-disasm --enable-iodebug
--enable-x86-debugger --with-x --with-x11
```

```
make
make install
```

## 制作image
```
bin/bximage -hd -mode="flat" -size=60 -q hd60M.img
```

## 导入mbr到image
```
dd if=./mbr.bin of=~/bochs/hd60M.img bs=512 count=1 conv=notrunc
```
