<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dirichlet hyperbola method](../../../../../../dirichlet-hyperbola-method.md) counts each factorization $n=ab$ once and gives, with $y=\lfloor\sqrt x\rfloor$,

$$
\sum_{n\leq x}\tau(n)
=\sum_{ab\leq x}1
=2\sum_{a\leq y}\left\lfloor\frac xa\right\rfloor-y^2.
$$

Using $\lfloor x/a\rfloor=x/a+O(1)$ and the [harmonic number](../../../../../../harmonic-number.md) estimate $H_y=\log y+\gamma+O(1/y)$, where $\gamma$ is the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md), we obtain

$$
\sum_{n\leq x}\tau(n)
=2x(\log y+\gamma)-y^2+O(y)
=x\log x+(2\gamma-1)x+O(\sqrt x).
$$

**Thus one may take $C=2\gamma-1$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
