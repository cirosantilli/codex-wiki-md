<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

Let $f$ be [continuous](../../../../../continuous-function.md) on a closed bounded interval $[a,b]$. First prove that $f$ is a [bounded function](../../../../../bounded-function.md). If it failed, we could choose $x_n\in[a,b]$ with $|f(x_n)|>n$. The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) gives a [subsequence](../../../../../subsequence.md) $x_{n_j}\to x_*$. Because the interval is closed, $x_*\in[a,b]$. [Continuity](../../../../../continuous-function.md) gives $f(x_{n_j})\to f(x_*)$, contradicting $|f(x_{n_j})|>n_j\to\infty$.

Now let $M=\sup\{f(x):x\in[a,b]\}$, which exists by [completeness of the real numbers](../../../../../completeness-of-the-real-numbers.md) and the bound just proved. Choose $y_n\in[a,b]$ with $f(y_n)>M-1/n$. A [convergent subsequence](../../../../../convergent-subsequence.md) has [limit of a sequence](../../../../../limit-of-a-sequence.md) $y_*\in[a,b]$, and [continuity](../../../../../continuous-function.md) gives $f(y_*)=M$. Applying the same argument to $-f$ gives attainment of the [infimum](../../../../../infimum.md). This proves the [extreme value theorem](../../../../../extreme-value-theorem.md): **the maximum and minimum both exist and are attained**. The argument also covers a one-point interval, where the conclusions are immediate.

## ↑ Ancestors (11)

1. [10C](../10c.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
