# Branch delay slot

↑ **Parent:** [MIPS architecture](mips-architecture.md)

In classic delayed-control-transfer MIPS, the instruction immediately after a branch or jump executes before control transfers. A harmless `sll $zero,$zero,0` can fill that slot. A jump-and-link records the address after this slot as its [return address](return-address.md).[Revision 2.00, JAL entry, p. 139](mips32-architecture-for-programmers-volume-ii-by-mips-technologies.md)

## ↑ Ancestors (4)

1. [MIPS architecture](mips-architecture.md)
2. [Instruction set architecture](instruction-set-architecture.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [MIPS architecture](mips-architecture.md)
- [MIPS instruction](mips-instruction.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/1/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/1/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/3/b/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
- [Pseudoinstruction](pseudoinstruction.md)
