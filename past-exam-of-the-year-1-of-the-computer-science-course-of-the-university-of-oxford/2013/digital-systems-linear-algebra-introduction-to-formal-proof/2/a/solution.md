<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [MIPS zero register](../../../../../mips-zero-register.md) as a [write-suppression destination](../../../../../write-suppression-destination.md): encode $r_d=0$. There are only 31 stored [processor registers](../../../../../processor-register.md), and address zero denotes the constant-zero source rather than a writable storage cell. Its writes are discarded, so

$$
\boxed{r_d=0\quad\Longrightarrow\quad\text{no visible register change}.}
$$

This permits a `store` to write memory while its unavoidable [register file](../../../../../register-file.md) write has no effect. It also implements a no-operation by selecting no memory write and destination zero. The statement that reads of register zero return zero is realized consistently by this standard constant-zero, discard-writes implementation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
