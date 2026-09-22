<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For order six, the support-midpoint sites are $x_i=i+3$, so

$$
(A_x)_{ij}=N_{j,6}(i+3)=N_{0,6}(i+3-j),\qquad0\le i,j\le n.
$$

By part (b), the complete finite [matrix](../../../../../../matrix.md) is the symmetric five-diagonal [matrix](../../../../../../matrix.md)

$$
\boxed{(A_x)_{ij}=\frac1{120}\begin{cases}
66,&i=j,\\26,&|i-j|=1,\\1,&|i-j|=2,\\0,&|i-j|>2.
\end{cases}}
$$

Only indices from $0$ through $n$ are retained; the first and last rows are truncated, with no exterior [coefficients](../../../../../../coefficient.md) or wraparound terms. For a row with all possible neighbors, the [strict diagonal dominance](../../../../../../strictly-diagonally-dominant-matrix.md) margin is $(66-26-26-1-1)/120=1/10$. Boundary rows have an equal or larger margin.

Here is the appropriate inverse estimate with its proof. If a square [matrix](../../../../../../matrix.md) $A$ has $|a_{ii}|-\sum_{j\ne i}|a_{ij}|\ge d>0$, choose an index $i$ maximizing $|z_i|$. The [reverse triangle inequality](../../../../../../reverse-triangle-inequality.md) gives

$$
|(Az)_i|\ge|a_{ii}|\,|z_i|-\sum_{j\ne i}|a_{ij}|\,|z_j|\ge d\|z\|_{\ell^\infty}.
$$

Thus $Az=0$ implies $z=0$, and a square finite [matrix](../../../../../../matrix.md) is invertible. Applying the same estimate with $z=A^{-1}b$ proves $\|A^{-1}b\|_{\ell^\infty}\le d^{-1}\|b\|_{\ell^\infty}$. The [inverse infinity-norm bound from diagonal dominance](../../../../../../inverse-infinity-norm-bound-from-diagonal-dominance.md) consequently yields

$$
\boxed{\|A_x^{-1}\|_{\ell^\infty}\le10.}
$$

This also proves existence and uniqueness of the requested interpolating spline for every data vector and every finite $n$. The [quintic cardinal spline midpoint collocation](../../../../../../quintic-cardinal-spline-midpoint-collocation.md) [matrix](../../../../../../matrix.md) includes the cases of one or two [coefficients](../../../../../../coefficient.md), where the dominance margin is even larger.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
