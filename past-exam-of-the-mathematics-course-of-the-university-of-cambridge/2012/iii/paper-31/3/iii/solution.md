<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Work with $z$ in the upper half-plane. Write the [Stieltjes matrix resolvents](../../../../../../stieltjes-matrix-resolvent.md) and their normalized [matrix traces](../../../../../../matrix-trace.md) as

$$
G=(X_N-zI)^{-1},\quad G^{(i)}=(X_N^{(i)}-zI)^{-1},\quad g=\frac1N\operatorname{Tr}G,\quad g^{(i)}=\frac1N\operatorname{Tr}G^{(i)},\quad q_i=x_i^TG^{(i)}x_i.
$$

The minor trace is normalized by $N$, not by $N-1$. This sign convention is the negative of the convention $(zI-X_N)^{-1}$ used in the general [resolvent of an operator](../../../../../../resolvent-of-an-operator.md) article. Here $g$ is the [Stieltjes transform of a measure](../../../../../../stieltjes-transform-of-a-measure.md) of the [empirical spectral measure](../../../../../../empirical-spectral-measure.md), with kernel $(x-z)^{-1}$.

The diagonal entries of $X_N$ are zero, so the preceding [Schur complement](../../../../../../schur-complement.md) formula gives $G_{ii}=-1/(z+q_i)$. Taking the [matrix trace](../../../../../../matrix-trace.md), subtracting the comparison value $-1/(z+g)$, and combining fractions gives the [resolvent self-consistency defect](../../../../../../resolvent-self-consistency-defect.md)

$$
\begin{aligned}\varepsilon_N(z)&=g+\frac1{z+g}\\&=\frac1N\sum_{i=1}^N\left(\frac1{z+g}-\frac1{z+q_i}\right)\\&=\boxed{\frac1N\sum_{i=1}^N\frac{q_i-g}{(z+g)(z+q_i)}}.\end{aligned}
$$

The positive numerator sign is fixed by this subtraction. All denominators are nonzero in the upper half-plane, as the imaginary-part estimate in the next part shows. The identity is deterministic and does not use entry independence or moment assumptions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
