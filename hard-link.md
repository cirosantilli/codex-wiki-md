# Hard link

↑ **Parent:** [File-system namespace](file-system-namespace.md)

A [directory entry](directory-entry.md) associating a name directly with an existing [file](computer-file.md). In the [inode](inode.md)-based example, successful `link("a", "b")` adds the second name for [inode](inode.md) 42 and increases its [hard link](hard-link.md) count from 1 to 2. Both [directory entries](directory-entry.md) have equal status; removing `a` leaves `b` usable. This example assumes both names are in the same [file system](file-system.md), the destination name is unused, and the operation is permitted. [The Open Group, POSIX.1-2017, link: adding a directory entry and incrementing the link count](https://pubs.opengroup.org/onlinepubs/9699919799/functions/link.html)

**Table of contents**

- [Unlinking an open file](unlinking-an-open-file.md)

## ↑ Ancestors (5)

1. [File-system namespace](file-system-namespace.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [File metadata](file-metadata.md)
- [File system](file-system.md)
- [Hard link](hard-link.md)
- [Inode](inode.md)
- [Open file description](open-file-description.md)
- [Operating system](operating-system.md)
- [POSIX](posix.md)
- [Symbolic link](symbolic-link.md)
- [Unlinking an open file](unlinking-an-open-file.md)
