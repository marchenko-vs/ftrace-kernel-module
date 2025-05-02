# Linux kernel module

## LKM for monitoring network traffic processed by specific process

Use Makefile to build kernel module.

For example, you want to monitor Mozilla Firefox. Then install module with

```bash
$ sudo insmod net_traffic.ko fname=firefox
```

After that start Mozilla Firefox and use it. Whenever you want you can check syslog by executing

```bash
$ sudo dmesg
```

In the end uninstall module with

```bash
$ sudo rmmod net_traffic
```

and check syslog again. You will see total network traffic processed by Firefox.

## Links

https://github.com/ilammy/ftrace-hook
