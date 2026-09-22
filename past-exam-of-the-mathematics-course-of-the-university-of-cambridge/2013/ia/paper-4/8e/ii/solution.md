<h1 id="8e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [prime-power contraction under pth powers](../../../../../../prime-power-contraction-under-pth-powers.md) is the key step. If $a=b+p^k h$ with $k\geq1$, the [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
a^p-b^p
=p^{k+1}hb^{p-1}
+\sum_{j=2}^{p}\binom pj p^{kj}h^j b^{p-j}.
$$

The first term is divisible by $p^{k+1}$. Each later term is also divisible by that power because $kj\geq k+1$ for $j\geq2$. This includes $p=2$ and $k=1$. Therefore

$$
a\equiv b\pmod{p^k}\quad\Longrightarrow\quad
a^p\equiv b^p\pmod{p^{k+1}}.
$$

Start with $x\equiv y\pmod{p^n}$ and apply this implication $r$ times, increasing both the exponent and modulus at each step:

$$
\boxed{x^{p^r}\equiv y^{p^r}\pmod{p^{n+r}}\qquad(r\geq0).}
$$

The case $r=0$ is precisely the original congruence.

By [Fermat's little theorem](../../../../../../fermat-little-theorem.md), $x^p\equiv x\pmod p$. Apply the same result with initial modulus $p$ and $r=n-1$:

$$
\boxed{x^{p^n}\equiv x^{p^{n-1}}\pmod{p^n}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
