# xv6 buffer cache

↑ **Parent:** [Buffer cache](buffer-cache.md)

The teaching implementation's `bget` checks device and block number under a shared [spinlock](spinlock.md), increments `refcnt` before releasing that lock, and then takes the buffer's content [mutex](mutex.md). On a [cache miss](cache-miss.md) it reserves an unused structure and clears `valid`; `bread` fills it only if necessary. This makes lookup and reservation share one [synchronization](synchronization-computing.md) boundary. `brelse` releases the content [mutex](mutex.md) and decrements the reference count. Unlike the stipulated trace policy, it moves the structure to the recent end only when that decrement reaches zero. [bio.c](xv6-risc-v-source-code/bio-c.md)

This implementation has `valid` and `refcnt` but no generic dirty flag. Its [file-system journaling](file-system-journaling.md) code records modified blocks with `log_write`, pins each newly recorded block, copies cached contents to the journal during commit, and unpins after installing the committed contents at their final locations. Thus journal pins keep modifications resident after callers release them. Its eviction loop does not perform the generic dirty-victim [buffer cache writeback](buffer-cache-writeback.md) of our model. [buf.h](xv6-risc-v-source-code/buf-h.md)[log.c](xv6-risc-v-source-code/log-c.md)

## ↑ Ancestors (5)

1. [Buffer cache](buffer-cache.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
