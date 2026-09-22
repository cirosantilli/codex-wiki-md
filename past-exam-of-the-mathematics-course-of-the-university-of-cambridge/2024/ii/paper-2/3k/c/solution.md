<h1 id="3k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes, for a binary code.** Correcting $e$ errors requires minimum distance at least $2e+1$. Apply the [parity extension](../../../../../../parity-extension.md): append to each word the bit that makes its total weight even. Every odd distance increases by one and every even distance is unchanged, so the extended minimum distance is at least $2e+2$. It therefore detects every pattern of at most $2e+1$ errors.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3K](../../3k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
