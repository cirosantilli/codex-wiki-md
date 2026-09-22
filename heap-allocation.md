# Heap allocation

↑ **Parent:** [Computer memory](computer-memory-split.md)

Heap allocation creates an [software object](software-object.md) whose lifetime need not match one lexical procedure call. Other [software objects](software-object.md) can retain references to it after the constructing call returns. Automatic storage reclamation therefore follows reachability or another memory-management discipline, rather than simply returning from that call.

**Table of contents**

- [Memory reclamation](memory-reclamation.md)
  - [Hazard pointer](hazard-pointer.md)
  - [Read-copy-update](read-copy-update.md)
    - [Grace period](grace-period.md)
  - [Use-after-free](use-after-free.md)

## ↑ Ancestors (3)

1. [Computer memory](computer-memory-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Heap memory](heap-memory.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-architecture/3/c/i/solution.md)
