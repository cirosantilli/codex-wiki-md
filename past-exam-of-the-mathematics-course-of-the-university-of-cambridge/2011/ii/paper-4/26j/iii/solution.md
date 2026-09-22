<h1 id="26j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The service-period arrival count has [probability generating function](../../../../../../probability-generating-function.md)

$$
\boxed{g(s)=\sum_{j\ge0}a_js^j=\int e^{-\lambda(1-s)t}\,dG(t),\qquad |s|\le1,}
$$

with $g(1)=1$ and $g'(1)=\rho$. Let $\Pi(s)=\sum_{j\ge0}\pi_js^j$. In stationarity the recurrence and independence give

$$
\Pi(s)=g(s)\left[\pi_0+\frac{\Pi(s)-\pi_0}{s}\right],
$$

initially for $0<s<1$. Rearrangement gives $\Pi(s)=\pi_0(s-1)g(s)/(s-g(s))$. Letting $s\uparrow1$ and using $\Pi(1)=1$ shows $\pi_0=1-\rho$. Hence

$$
\boxed{\Pi(s)=\frac{(1-\rho)(s-1)g(s)}{s-g(s)}.}
$$

Analytic continuation gives the identity inside the unit disc; boundary values follow by convergence of the probability series, with removable limiting values wherever the displayed quotient is indeterminate, particularly at $s=1$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
