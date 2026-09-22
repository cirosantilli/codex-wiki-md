<h1 id="11g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an odd prime $p$, the [Legendre symbol](../../../../../../legendre-symbol.md) is

$$
\left(\frac ap\right)=
\begin{cases}
0,&p\mid a,\\
1,&a\not\equiv0\pmod p\text{ is a quadratic residue},\\
-1,&a\text{ is a quadratic nonresidue}.
\end{cases}
$$

[Euler criterion](../../../../../../euler-criterion.md) states that

$$
\boxed{
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.}
$$

If $p\mid a$, both sides vanish. Otherwise choose a [primitive root](../../../../../../primitive-root-modulo-n.md) $g$ and write $a\equiv g^m$. Since $g^{(p-1)/2}\equiv-1$,

$$
a^{(p-1)/2}\equiv(-1)^m.
$$

The power $g^m$ is a square exactly when $m$ is even, proving the criterion. Taking $a=-1$ gives the [first supplementary law for quadratic reciprocity](../../../../../../first-supplementary-law-for-quadratic-reciprocity.md)

$$
\boxed{\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
