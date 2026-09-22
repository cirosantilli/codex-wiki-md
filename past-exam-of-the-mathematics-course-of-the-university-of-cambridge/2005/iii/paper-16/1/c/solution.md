<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The equation $\sigma^n x=x$ says $x_{r+n}=x_r$ for every $r\in\mathbb Z$. Thus a solution is determined uniquely by the block $(x_0,\ldots,x_{n-1})$, repeated in both directions. It belongs to the [subshift of finite type](../../../../../../subshift-of-finite-type.md) exactly when all transitions inside the block, and the closing transition from $x_{n-1}$ to $x_0$, are allowed. Hence these [fixed points](../../../../../../fixed-point.md) of the $n$th [iteration of a map](../../../../../../iterated-function.md) are in [bijection](../../../../../../bijection.md) with the closed transition chains of $n$ steps with a specified symbol at time zero. By the counting argument in part (b), the number starting at $i$ is $(A^n)_{ii}$. Summing over $i$ proves the [trace formula for periodic points of a subshift](../../../../../../trace-formula-for-periodic-points-of-a-subshift.md):

$$
\boxed{\#\operatorname{Fix}(\sigma^n)=\operatorname{tr}(A^n).}
$$

Every closed transition chain extends by periodic repetition, so the extension issue in part (b) does not affect this formula. We count points, not [periodic orbits](../../../../../../periodic-orbit.md): a least-period-$d$ [periodic orbit](../../../../../../periodic-orbit.md) contributes its $d$ distinct points.

**Here period $n$ means fixed by $\sigma^n$, so the least period may divide $n$.** If $P_d$ denotes the number of points of least period exactly $d$, division with remainder shows that a point is fixed by $\sigma^n$ exactly when its least period divides $n$. Consequently

$$
\operatorname{tr}(A^n)=\sum_{d\mid n}P_d,qquad
P_n=\sum_{d\mid n}\mu_{\mathrm M}(n/d)\operatorname{tr}(A^d),
$$

where $\mu_{\mathrm M}$ is the [Möbius function](../../../../../../mobius-function.md) and the second equality is [Möbius inversion](../../../../../../mobius-inversion-formula.md). For example, $A=(1)$ has one point fixed by every power but no point of least period two; interpreting the printed formula as an exact-period count would therefore be false.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
