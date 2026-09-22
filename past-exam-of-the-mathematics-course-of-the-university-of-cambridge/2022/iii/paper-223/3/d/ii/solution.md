<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $d<c$. Directly comparing the two piecewise densities gives

$$
\frac{g_1(x)}{g_0(x)}=
\begin{cases}
d,&r(x)\leq d,\\
r(x),&d<r(x)<c,\\
c,&r(x)\geq c.
\end{cases}
$$

Since

$$
\log r(x)=\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right),
$$

we obtain

$$
\log\frac{g_1(x)}{g_0(x)}
=\left[\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right)\right]_{\log d}^{\log c}.
$$

**Thus the sample log-likelihood ratio is $nS_n$ with truncation values $a=\log d$ and $b=\log c$. Rejecting for large $S_n$ is exactly the likelihood-ratio test between the two least-favorable contaminated distributions.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 223](../../../../paper-223-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
