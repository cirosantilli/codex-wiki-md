<h1 id="11g/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First handle possible zero values. If $d_m=d_n=0$, the previous upper bound forces $x_m=x_n$. Thus, if infinitely many $d_m$ vanish, choosing those indices gives a constant [subsequence](../../../../../../../subsequence.md), which satisfies both inequalities.

Otherwise, discard the finitely many zero values and use $d_m\to0$ to choose increasing indices $k_j$ with

$$
\delta_j:=d_{k_j}>0,\qquad \delta_{j+1}\leq\delta_j/8.
$$

Set $y_j=x_{k_j}$. The preceding bounds give $|\delta_j-\delta_\ell|\leq d(y_j,y_\ell)\leq\delta_j+\delta_\ell$. For $m\geq2$,

$$
\frac{d(y_{m+1},y_m)}{d(y_m,y_{m-1})}\leq\frac{(9/8)\delta_m}{(7/8)\delta_{m-1}}\leq\frac9{56}<\frac13.
$$

For $m<n$, use $\delta_n\leq\delta_m/8$ and $\delta_{n+1}\leq\delta_m/64$ to obtain

$$
\frac{d(y_{m+1},y_{n+1})}{d(y_m,y_n)}\leq\frac{\delta_m/8+\delta_m/64}{(7/8)\delta_m}=\frac9{56}<\frac12.
$$

The same holds when $n<m$ by symmetry; when $m=n$, both distances are zero. This proves **both required inequalities**. The adjacent-distance inequality is understood for $m\geq2$, since this [subsequence](../../../../../../../subsequence.md) starts at index one and has no $y_0$.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [11G](../../../11g.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
