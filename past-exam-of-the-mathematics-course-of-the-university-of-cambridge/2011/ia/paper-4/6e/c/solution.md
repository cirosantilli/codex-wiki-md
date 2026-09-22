<h1 id="6e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $p=3k+2$. A solution has $p\nmid x$, so [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives

$$
1\equiv x^{p-1}=x^{3k+1}=(x^3)^kx\equiv(-1)^kx\pmod p.
$$

Thus $x\equiv(-1)^k\pmod p$. If $p$ is odd, then $k$ is odd and $x\equiv-1$. The remaining [prime](../../../../../../prime-number.md) case $p=2$ has $k=0$ and $x\equiv1\equiv-1\pmod2$ as well. Since $-1$ itself always satisfies the equation, **the unique solution is $x\equiv-1\pmod p$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
