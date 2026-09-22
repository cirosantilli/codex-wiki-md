<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $S^n$ as the union of slightly enlarged northern and southern hemispheres $U$ and $V$. Both are [contractible](../../../../../contractible-space.md), while $U\cap V$ deformation retracts onto $S^{n-1}$. The reduced [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) therefore gives

$$
\widetilde H_i(S^n;\mathbb Z)\cong\widetilde H_{i-1}(S^{n-1};\mathbb Z).
$$

Starting from $\widetilde H_0(S^0;\mathbb Z)\cong\mathbb Z$ proves the [homology of a sphere](../../../../../homology-of-a-sphere.md):

$$
H_i(S^n;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,n,\\
0,&\text{otherwise}.
\end{cases}
$$

This uses no [cellular homology](../../../../../cellular-chain-complex.md). A reflection of $S^n$ reverses its orientation and has [degree of a continuous mapping](../../../../../degree-of-a-continuous-mapping.md) $-1$, so it induces the identity on $H_0$, multiplication by $-1$ on $H_n$, and the unique map between zero groups in every other degree.

For a [CW complex](../../../../../cw-complex.md) with skeleta $X^k$, its [cellular chain complex](../../../../../cellular-chain-complex.md) is

$$
C_k^{\mathrm{cell}}(X)=H_k(X^k,X^{k-1};\mathbb Z)\cong\bigoplus_{\text{$k$-cells}}\mathbb Z.
$$

The differential is the connecting map to $H_{k-1}(X^{k-1})$ followed by passage to $H_{k-1}(X^{k-1},X^{k-2})$. Equivalently, the coefficient of a $(k-1)$-cell in the boundary of a $k$-cell is the [degree](../../../../../degree-of-a-continuous-mapping.md) obtained from its attaching map after collapsing the complement of that lower cell. This is the [cellular boundary formula](../../../../../cellular-boundary-formula.md).

The quotient $D^k/(x\sim-x\text{ on }S^{k-1})$ builds $\mathbb{RP}^k$ from $\mathbb{RP}^{k-1}$ by one $k$-cell, so $\mathbb{RP}^n$ has one cell in each dimension $0,\ldots,n$. The two lifts of the attaching map contribute with relative sign $(-1)^k$, and the [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) has differential

$$
d_k=1+(-1)^k=
\begin{cases}
0,&k\text{ odd},\\
2,&k\text{ even}.
\end{cases}
$$

Consequently

$$
H_i(\mathbb{RP}^n;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,\\
\mathbb Z/2,&0<i<n\text{ and }i\text{ odd},\\
\mathbb Z,&i=n\text{ and }n\text{ odd},\\
0,&\text{otherwise}.
\end{cases}
$$

With $\mathbb F_2=\mathbb Z/2$ coefficients every differential vanishes, and hence

$$
\boxed{H_i(\mathbb{RP}^n;\mathbb F_2)\cong\mathbb F_2\quad(0\leq i\leq n),}
$$

with zero homology outside that range.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
