# Symbolic link

↑ **Parent:** [File-system namespace](file-system-namespace.md)

A separate [file](computer-file.md) containing a path string to be interpreted during lookup. A [symbolic link](symbolic-link.md) to `a` stores that spelling rather than adding another [hard link](hard-link.md) to [inode](inode.md) 42; it can remain after `a` disappears and then fail to reach a target. It does not increase the target's [hard link](hard-link.md) count. The diagrams below track only [hard links](hard-link.md) and open references. [The Open Group, POSIX, symlink: storing the supplied path string](https://pubs.opengroup.org/onlinepubs/009695299/functions/symlink.html)

// Target: computer-science.bigb

## ↑ Ancestors (5)

1. [File-system namespace](file-system-namespace.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Computer file](computer-file.md)
- [Symbolic link](symbolic-link.md)
