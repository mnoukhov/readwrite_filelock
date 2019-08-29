# Read/Write FileLock
Wrapper on [filelock](https://github.com/benediktschmitt/py-filelock) to allow for multiple read accesses but maintain a write lock. Currently implements a fair lock with neither write nor read priority.

Inspired by the very nice [readerwriterlock](https://github.com/elarivie/pyReaderWriterLock)

## Why

This is useful when you want to use locks in a distributed setting without being ableto use `notify` or have a centralized process that maintain the number of active readers

## How to use

The interface is exactly like `FileLock`

