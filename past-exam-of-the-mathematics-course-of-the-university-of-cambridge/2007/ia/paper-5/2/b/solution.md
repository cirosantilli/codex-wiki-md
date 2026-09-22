<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Both kinds of [context switch](../../../../../../context-switch.md) save and restore registers, a program counter, stack pointer and scheduler state. Switching between [operating-system processes](../../../../../../process-computing.md) additionally changes the address-space and protection context, including the page-table root. Cached translations must be invalidated or distinguished by address-space identifiers, and the new process may have a different memory and cache locality.

[Software threads](../../../../../../thread-computing.md) of one process share its address space and most resources, so a thread switch normally preserves the page-table root and valid cached translations; only the execution context, stack and thread-specific state need change. Thus **a process switch requires address-space management which a same-process thread switch usually avoids**. Tagged translation caches can reduce the extra cost, so a complete [translation lookaside buffer](../../../../../../translation-lookaside-buffer.md) flush is not an inevitable feature of every process switch.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
