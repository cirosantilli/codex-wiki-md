<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

In the multiplicative [group](../../../../../group-split.md) $\mathbb F_p^\times$, the squaring map is a [group homomorphism](../../../../../group-homomorphism.md) with kernel $\{1,-1\}$, since $p$ is odd. Every nonzero square therefore has exactly two square roots. There are $(p-1)/2$ [quadratic residues](../../../../../quadratic-residue.md) and the same number of nonresidues, and consequently $\sum_{a=1}^{p-1}\left(\frac ap\right)=0$.

For $nm_n\equiv1\pmod p$, direct multiplication gives $n^2(1+m_n)\equiv n^2+n=n(n+1)$. Multiplicativity of the [Legendre symbol](../../../../../legendre-symbol.md), including its value zero on multiples of $p$, implies

$$
\left(\frac{n(n+1)}p\right)=\left(\frac{1+m_n}p\right).
$$

Inversion permutes $\mathbb F_p^\times$, so $1+m_n$ runs through all residue classes except $1$. Thus

$$
\boxed{\sum_{n=1}^{p-1}\left(\frac{n(n+1)}p\right)=\sum_{a\in\mathbb F_p,\ a\ne1}\left(\frac ap\right)=0-1=-1.}
$$

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
