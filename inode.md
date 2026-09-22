# Inode

↑ **Parent:** [File system](file-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inode)

An [inode](inode.md) is a [data structure](data-structure.md) describing an object in an [inode](inode.md)-based [file system](file-system.md). For an ordinary [file](computer-file.md), it records [file metadata](file-metadata.md) such as type, owner, access permissions, size and [hard link](hard-link.md) count, together with information locating the contents. In the direct-reference toy layout, [inode](inode.md) 42 points to [file data blocks](file-data-block.md) 7 and 9; its two names `a` and `b` live in [directory entries](directory-entry.md). Other [file systems](file-system.md) can locate contents differently, so the diagram is a model of the separation rather than a universal storage layout. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 40, sections 40.3–40.4: inodes and directory organization](https://pages.cs.wisc.edu/~remzi/OSTEP/file-implementation.pdf)

An [inode](inode.md) number is unique only within its [file system](file-system.md) among allocated objects. Two different [file systems](file-system.md) can each have [inode](inode.md) 42, referring to unrelated [files](computer-file.md). [POSIX](posix.md) exposes the [file system](file-system.md)'s device identity as `st_dev` and the [file](computer-file.md)'s serial number as `st_ino`; the pair identifies a [file](computer-file.md) within a running system. Neither the bare [inode](inode.md) number nor that pair is a permanent historical identifier: after reclamation, a later [file](computer-file.md) can reuse the number. In particular, comparing an old saved number with a new one does not establish continuity of the [file](computer-file.md). [The Open Group, POSIX.1-2017, sys/stat.h: joint identity from st\_dev and st\_ino](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/sys_stat.h.html)

The design's appeal is that one [inode](inode.md) unifies the [file metadata](file-metadata.md) and contents reached through several [directory entries](directory-entry.md). Ritchie and Thompson's original 1974 account explicitly describes a [directory entry](directory-entry.md) as a name and an i-number, with the corresponding [inode](inode.md) holding ownership, protection, size, content addresses and the [hard link](hard-link.md) count. It gives a concrete early explanation of how names and [file](computer-file.md) identity can evolve separately. [Ritchie and Thompson, The UNIX Time-Sharing System, 1974, section 4: implementation of the file system](https://www.cs.cmu.edu/~15712/papers/ritchie74.pdf)

// Target: computer-science.bigb

## ↑ Ancestors (4)

1. [File system](file-system.md)
2. [Operating system](operating-system.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Buffer cache](buffer-cache.md)
- [Directory entry](directory-entry.md)
- [File data block](file-data-block.md)
- [File descriptor](file-descriptor.md)
- [File metadata](file-metadata.md)
- [File system](file-system.md)
- [File-system directory](file-system-directory.md)
- [File-system journaling](file-system-journaling.md)
- [File-system namespace](file-system-namespace.md)
- [File-system transaction](file-system-transaction.md)
- [Hard link](hard-link.md)
- [Inode](inode.md)
- [Inode allocation bitmap](inode-allocation-bitmap.md)
- [Kernel (operating system)](kernel-operating-system.md)
- [Linux kernel](linux-kernel.md)
- [Open file description](open-file-description.md)
- [Operating system](operating-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/8/d/solution.md)
- [POSIX](posix.md)
- [Symbolic link](symbolic-link.md)
- [Unlinking an open file](unlinking-an-open-file.md)
