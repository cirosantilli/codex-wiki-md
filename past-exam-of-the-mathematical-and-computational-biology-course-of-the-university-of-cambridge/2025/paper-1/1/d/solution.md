<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With its default argument and a nonnegative [integer](../../../../../integer-split.md) input, it prints the decimal [digits](../../../../../numerical-digit.md) of $n$ in order, one per line. For example, `mystery4(407)` prints **`4`, then `0`, then `7`**. [Integer division](../../../../../integer-division.md) removes the final [digit](../../../../../numerical-digit.md), [recursion](../../../../../recursion-computer-science.md) handles the preceding [digits](../../../../../numerical-digit.md), and the [remainder](../../../../../remainder.md) gives the final [digit](../../../../../numerical-digit.md). The function returns `None`.

There is a subtlety for a nondefault base: the recursive call omits `m`, so it resets to $10$. For $m\ge2$ and $n\ge m$, the actual output is the decimal [digits](../../../../../numerical-digit.md) of $\lfloor n/m\rfloor$, followed by the [remainder](../../../../../remainder.md) $n\bmod m$. For example, `mystery4(13, 2)` prints **`6`, then `1`**, rather than the binary [digits](../../../../../numerical-digit.md) of $13$. Passing `m` on to the recursive call would give a consistent base-$m$ [positional notation](../../../../../positional-notation.md). The interpretation as [digits](../../../../../numerical-digit.md) assumes $n\ge0$ and $m\ge2$; arbitrary [integer](../../../../../integer-split.md) arguments need not satisfy those conditions.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
