### Introducción a los módulos del kernel
Universidad ICESI  
Curso: Sistemas Operativos  
Docente: Daniel Barragán C.  
Tema: Introducción a las llamadas al sistema  
Correo: daniel.barragan at correo.icesi.edu.co

### Objectives

* Learn what a kernel module is and how to load them

### Description

Kernel modules allow you to introduce changes in the operating system without compiling all the kernel sources

#### Load a kernel module

```
# git clone https://github.com/jvns/kernel-module-fun.git
# cd kernel-module-fun

# UNAME=$(uname -r)
# yum install gcc kernel-devel-${UNAME%.*}
# make all
# sudo insmod hello.ko
# dmesg | tail

# lsmod
```

### References
https://github.com/jvns/kernel-module-fun.git  
https://jvns.ca/blog/2014/09/18/you-can-be-a-kernel-hacker/  
http://blog.csdn.net/u012343297/article/details/79141878
