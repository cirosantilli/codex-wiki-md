<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [divided difference](../../../../../../divided-difference.md) is a finite linear combination of [spline knot](../../../../../../spline-knot.md) values, so it commutes with the finite integral. For every [spline knot](../../../../../../spline-knot.md) $t_j$ in the defining interval,

$$
\int_{t_i}^{t_{i+k}}(t_j-t)_+^{k-1}\,dt=\frac{(t_j-t_i)^k}{k}.
$$

It follows that

$$
\int_{t_i}^{t_{i+k}}M_i(t)\,dt=[t_i,\ldots,t_{i+k}](u-t_i)^k=1,
$$

because the order-$k$ [divided difference](../../../../../../divided-difference.md) of a monic degree-$k$ [polynomial](../../../../../../polynomial-split.md) is its leading coefficient. This proves the [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md).

For the [partition of unity](../../../../../../partition-of-unity.md), let $N_{i,r}$ denote the partition-normalized order-$r$ [B-spline](../../../../../../b-spline.md). The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) is

$$
N_{i,r}(t)=\frac{t-t_i}{t_{i+r-1}-t_i}N_{i,r-1}(t)+\frac{t_{i+r}-t}{t_{i+r}-t_{i+1}}N_{i+1,r-1}(t).
$$

It follows by substituting the explicit [divided difference](../../../../../../divided-difference.md) formula into both sides and collecting each [truncated power function](../../../../../../truncated-power-function.md). The starting case is $N_{i,1}=\mathbf1_{[t_i,t_{i+1})}$, with endpoint conventions irrelevant when $r\ge2$. The two weights are nonnegative wherever their respective lower-order [B-splines](../../../../../../b-spline.md) are nonzero. Induction therefore gives $N_{i,r}\ge0$ and strict positivity in its open [support](../../../../../../support.md).

Extend the finite [spline knot sequence](../../../../../../spline-knot-sequence.md) strictly in both directions, with no finite accumulation. At each point only finitely many [B-splines](../../../../../../b-spline.md) are nonzero. For the full extended family the sum is one for order one. Summing the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md), the combined coefficient of $N_{j,r-1}$ is

$$
\frac{t-t_j}{t_{j+r-1}-t_j}+\frac{t_{j+r-1}-t}{t_{j+r-1}-t_j}=1.
$$

Induction gives a full [partition of unity](../../../../../../partition-of-unity.md) at every order. On $t_k<t<t_{n+1}$, all extended order-$k$ [functions](../../../../../../function-split.md) with index $i\le0$ or $i\ge n+1$ vanish by their supports. Hence

$$
\boxed{\sum_{i=1}^nN_i(t)=1\quad(t_k<t<t_{n+1}),\qquad\int M_i=1.}
$$

The same argument gives the useful global [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md), $0\le\sum_{i=1}^nN_i(t)\le1$, including outside the basic [spline knot](../../../../../../spline-knot.md) interval.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
