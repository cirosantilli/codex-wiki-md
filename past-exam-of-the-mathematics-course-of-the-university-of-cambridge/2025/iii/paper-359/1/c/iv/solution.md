<h1 id="1/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $u$ and $v$ be two weak solutions with the same initial value, and put $w=u-v$. Bilinearity gives

$$
w_t+\nu Aw+B(P_Nu,w)+B(P_Nw,v)=0.
$$

Pair with $w$. The first transport term vanishes because $P_Nu$ is divergence free. Part a and the [Young inequality](../../../../../../../young-s-inequality-for-products.md) give

$$
\begin{aligned}
|\langle B(P_Nw,v),w\rangle|
&\leq c\lambda_N^{1/4}|w|\,\|v\|\,\|w\|\\
&\leq\frac\nu2\|w\|^2
+\frac{c^2\lambda_N^{1/2}}{2\nu}
\|v\|^2|w|^2.
\end{aligned}
$$

Therefore

$$
\frac d{dt}|w|^2+\nu\|w\|^2
\leq\frac{c^2\lambda_N^{1/2}}{\nu}
\|v\|^2|w|^2.
$$

The coefficient is integrable because $v\in L^2(0,T;V)$. Since $w(0)=0$, the [Gronwall inequality](../../../../../../../gronwall-inequality.md) gives $w=0$ on $[0,T]$. The global weak solution is unique.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
