<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [inverse theorem for trigonometric approximation](../../../../../../inverse-theorem-for-trigonometric-approximation.md) gives

$$
\omega(f,n^{-1})\leq\frac Cn\sum_{\nu=0}^nE_\nu(f).
$$

Summing $\nu^{-\alpha}$ proves

$$
\boxed{\omega(f,n^{-1})=
\begin{cases}O(n^{-\alpha}),&0<\alpha<1,\\O(n^{-1}\log n),&\alpha=1.\end{cases}}
$$

For $c_k=a^{-k}$, part (a) gives $E_n(g)\asymp a^{-m}\asymp n^{-\log_5a}$. If $a<5$, an increment $h=\pi/5^{m+2}\leq1/n$ at $x=0$ has nonnegative summands and its $k=m+2$ term is $\asymp n^{-\log_5a}$. Part (c) handles $a=5$. Therefore

$$
\boxed{\omega(g,n^{-1})\asymp
\begin{cases}n^{-\log_5a},&1<a<5,\\n^{-1}\log n,&a=5.\end{cases}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
