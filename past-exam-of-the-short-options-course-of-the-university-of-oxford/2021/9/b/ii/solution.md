<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $f(X,Y)=X[r/(1+bY^2)-\delta]$. At the positive [steady state](../../../../../steady-state.md), $1+b(N^*)^2=r/s$, where $s=\delta+1$. The two [partial derivatives](../../../../../partial-derivative.md) are

$$
f_X(N^*,N^*)=1,\qquad f_Y(N^*,N^*)=-\frac{2rb(N^*)^2}{(1+b(N^*)^2)^2}=-\frac{2s(r-s)}r.
$$

The first-order [Taylor expansion](../../../../../taylor-expansion.md) with $N_t=N^*+n_t$ therefore gives

$$
\boxed{n_{t+1}-n_t+a n_{t-1}=0,\qquad a=\frac{2s(r-s)}r=\frac{2(r-(\delta+1))(\delta+1)}r.}
$$

Equivalently, the [linearization](../../../../../linearization.md) on $(n_t,n_{t-1})$ has matrix $\begin{pmatrix}1&-a\\1&0\end{pmatrix}$ and [characteristic polynomial](../../../../../characteristic-polynomial.md) $\mu^2-\mu+a$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
