# Write-suppression destination

↑ **Parent:** [Register file](register-file.md)

A destination code whose writes have no architectural effect. Replacing a disabled write by a write to such a destination can remove a global register-file enable input: every actual register enable becomes its address-decode line, and the suppression code activates none. The instruction control must still select that code whenever a write should be suppressed. This transformation preserves the register-state update, rather than making the control decision unnecessary.

## ↑ Ancestors (5)

1. [Register file](register-file.md)
2. [Processor register](processor-register.md)
3. [Central processing unit](central-processing-unit.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [MIPS zero register](mips-zero-register.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/digital-systems-linear-algebra-introduction-to-formal-proof/3/b/i/solution.md)
