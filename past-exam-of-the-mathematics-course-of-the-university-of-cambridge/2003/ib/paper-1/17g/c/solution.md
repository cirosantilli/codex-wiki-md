<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $n$ is nonzero modulo $p$, it has a unique multiplicative inverse $m$ in the nonzero residues. The inverse cannot be $-1$ because that would imply $n=-1$, excluded by the range. Thus $1\leq m\leq p-2$ as claimed. The congruence $mn=1$ gives

$$
n(n+1)=n^2(1+m)\pmod p.
$$

The [Legendre symbol](../../../../../../legendre-symbol.md) of the nonzero square $n^2$ is one. Using [multiplicativity of the Legendre symbol](../../../../../../multiplicativity-of-the-legendre-symbol.md) therefore gives

$$
\boxed{\left(\frac{n(n+1)}p\right)=\left(\frac{1+m}p\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
