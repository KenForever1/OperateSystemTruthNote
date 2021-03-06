# 库函数是用户进程与内核的桥梁

```
gcc -v -o main.bin main.c
```

```
./main.bin
```

```
gcc -E main.c
```


```
ltrace -S ./main.bin
```

```
strace ./main.bin

strace -e trace=write ./main.bin
```
