<h1 id="20g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\alpha=\sqrt[n]{m}$ and $\zeta=e^{2\pi i/n}$. The $n$ [field embeddings](../../../../../../field-embedding.md) of $L$ into $\mathbb C$ send $\alpha$ to $\zeta^j\alpha$, so the [field trace](../../../../../../field-trace.md) is

$$
\operatorname{Tr}_{L/\mathbb Q}(\alpha^r)
=\alpha^r\sum_{j=0}^{n-1}\zeta^{jr}
=\begin{cases}
n,&r=0,\\
nm,&r=n,\\
0,&1\leq r\leq2n-2,\ r\ne n.
\end{cases}
$$

For the [trace pairing](../../../../../../trace-pairing.md) $T(x,y)=\operatorname{Tr}_{L/\mathbb Q}(xy)$, the basis $\beta_i=\alpha^i$ therefore has [dual basis](../../../../../../dual-basis.md)

$$
\boxed{\beta_0^*=\frac1n,
\qquad
\beta_i^*=\frac{\alpha^{n-i}}{nm}\quad(1\leq i\leq n-1)}.
$$

Every element of $\mathbb Z[\alpha]$ is an [algebraic integer](../../../../../../algebraic-integer.md). If $x\in\mathcal O_L$ and $z\in\mathbb Z[\alpha]$, then $xz$ is an algebraic integer and its trace is an [integer](../../../../../../integer.md). Thus $x$ belongs to the [trace-dual lattice](../../../../../../trace-dual-lattice.md) of $\mathbb Z[\alpha]$, which is generated over $\mathbb Z$ by the displayed dual basis. Since $1/n=m/(nm)$, every such linear combination lies in $(nm)^{-1}\mathbb Z[\alpha]$. Hence

$$
\boxed{\mathcal O_L\subseteq\frac1{nm}\mathbb Z[\sqrt[n]{m}]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20G](../../20g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
