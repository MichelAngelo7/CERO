verify the dependecy of file 
ldd hello

show call library of file
ltrace hello

____Ring3 or usermode______   call      ___ring0 or Kernelmode___
| executable | --> |Library|   -->      |         Kernel         |
--------------     --------             -------------------------

view syscalls

strace ./hello


EXEC -> LIB -> KERNEL (SYSCALLS)


less /proc/cpuinfo

desassember

objdump -d hello | less

/main

hello.py -> /usr/bin/python -> printf /puts -> libc -> write 