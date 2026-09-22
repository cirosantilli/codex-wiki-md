<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At $2$ there is [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), and the [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md) gives an [exact sequence](../../../../../../exact-sequence.md)

$$
0\longrightarrow E_1(\mathbb Q_2)\longrightarrow E(\mathbb Q_2)\longrightarrow\widetilde E_2(\mathbb F_2)\longrightarrow0.
$$

The quotient has order $5$ and is consequently a [cyclic group](../../../../../../cyclic-group.md). For every odd integer $n$, multiplication by $n$ is an automorphism of $E_1(\mathbb Q_2)$: its [formal group law](../../../../../../formal-group-law.md) has multiplication series $nt+O(t^2)$ with unit linear coefficient, whose inverse [formal power series](../../../../../../formal-power-series.md) has integral coefficients and converges on $2\mathbb Z_2$. This is the [prime-to-residue-characteristic multiplication on a formal group](../../../../../../prime-to-residue-characteristic-multiplication-on-a-formal-group.md).

Thus the odd-primary [torsion subgroup](../../../../../../torsion-subgroup.md) injects into the order-five quotient. It also realizes that quotient: choose a lift $P$ of any reduced point, so $[5]P\in E_1$. There is a unique $Q\in E_1$ with $[5]Q=[5]P$. Then $P-Q$ is killed by five and has the prescribed reduction. This proves the [prime-to-p torsion lifts uniquely at good reduction](../../../../../../prime-to-p-torsion-lifts-uniquely-at-good-reduction.md) directly here. Therefore, for an odd prime $p$,

$$
\boxed{E(\mathbb Q_2)[p^\infty]\cong\begin{cases}\mathbb Z/5\mathbb Z,&p=5,\\0,&p\ne5.\end{cases}}
$$

The five-primary subgroup consists of the unique five-torsion lifts of the five reduced points. These lifts need not be rational over $\mathbb Q$; the preceding answer about rational [torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) does not contradict their existence over the [p-adic field](../../../../../../p-adic-field.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
