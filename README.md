# A Kernel Seedling
In this lab, I modified a program so it counts the current number of running processes.

## Building
```shell
Command for build: make
```

## Running
```shell
Command for running binary: sudo insmod proc_count.ko
```
# Result: this command was successful and did not print any error messages.
# running the command sudo dmesg -l info lists additional info abt the kernel activity.

## Cleaning Up
```shell
Command for cleaning the built binary: make clean
```

## Testing
```python
python -m unittest
```
Result: OK (all tests passed), approximately 160 processes running

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
kernel version tested on: Linux 5.14.8-arch1-1 #1 SMP PREEMPT