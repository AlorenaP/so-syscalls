### Introducción a las llamadas al sistema
Universidad ICESI  
Curso: Sistemas Operativos  
Docente: Daniel Barragán C.  
Tema: Introducción a las llamadas al sistema  
Correo: daniel.barragan at correo.icesi.edu.co

### Introduction
In computing, a system call is how a program requests a service from an operating system's kernel. This may include hardware-related services (for example, accessing a hard disk drive), creation and execution of new processes, and communication with integral kernel services such as process scheduling. System calls provide an essential interface between a process and the operating system.

![][1]

More info: [**Syscall from A to Z**][linuxorg-syscalls]

### Objectives
* Learn the difference between interpreted and compiled languages
* Learn how to use syscalls from C source code
* Learn how to use syscalls related with process management

### Description

In the souces folder you can find the source code in c language for practicing different syscals.  

In order to compile the sources you can execute the following command:

```
$ make ejemplo_01
```

or

```
$ chmod u+x compilar_ejecutar
$ ./compilar_ejecutar.sh syscl_01
```

#### syscl_1.c

This is the source code of a hello world application written in C language

#### syscl_2.c

This is the source code of a basic application that employs the getpid() system call to return its
process id

### Activities

Compile and explain the sources from syscl_3.c to syscl_11.c

[linuxorg-syscalls]: https://notes.shichao.io/lkd/ch1/
[1]: images/syscalls.png
