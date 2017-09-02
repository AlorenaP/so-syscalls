### Introducción al uso de strace
Universidad ICESI  
Curso: Sistemas Operativos  
Docente: Daniel Barragán C.  
Tema: Introducción a las llamadas al sistema  
Correo: daniel.barragan at correo.icesi.edu.co

### Objectives
* Learn to trace applications from syscalls

### Description
Strace is an application that allows you to find the syscalls that are called when you execute a process in the operating system

#### Install strace

Install dependency
```
# yum install strace
```

#### Trace some applications

The most simple linux binary
```
# strace -etrace=exit_group /usr/bin/true
```

Test with a call that uses sockets
```
# strace -etrace=sendto ping -c 1 127.0.0.1
```

There are three standard file descriptions, STDIN, STDOUT, and STDERR. They are assigned to 0, 1, and 2 respectively.

#### Trace python applications

The most simple python test with syscalls
```
# strace python -c ""
```

**mistery1.py**
```
print("hello syscalls")
```

```
# strace -etrace=write python mistery1.py
```

### References

https://linuxmeerkat.wordpress.com/2011/12/02/file-descriptors-explained/
http://man7.org/linux/man-pages/man2/write.2.html
