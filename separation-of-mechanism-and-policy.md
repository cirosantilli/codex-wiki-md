# Separation of mechanism and policy

↑ **Parent:** [Operating system](operating-system.md)

Distinguishing the operations a system can enforce from the choices about how to use them. In a [microkernel](microkernel.md), a protected [IPC](inter-process-communication.md) operation can deliver requests while a [user-space service](user-space-service.md) decides which [files](computer-file.md) a caller may read. The division is a design choice: every real mechanism still has rules and limits.

## ↑ Ancestors (3)

1. [Operating system](operating-system.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Microkernel](microkernel.md)
- [Microkernel file-read example](microkernel-file-read-example.md)
