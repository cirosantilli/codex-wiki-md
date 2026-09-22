<h1 id="27h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Regard the same triangular functions as cutoffs in the frequency variable. They satisfy

$$
0\leq\theta_n(\xi)\uparrow1.
$$

Since $\widehat f\geq0$, monotone convergence gives

$$
\|\widehat f\|_1
=\lim_{n\to\infty}\int_{\mathbb R}\theta_n(\xi)\widehat f(\xi)\,d\xi.
$$

Fubini's theorem and evenness of $\theta_n$ give

$$
\int\theta_n(\xi)\widehat f(\xi)\,d\xi
=\int f(x)\widehat\theta_n(x)\,dx.
$$

Part (b) shows that $\widehat\theta_n\geq0$. Moreover, Fourier inversion at zero yields

$$
\int_{\mathbb R}\widehat\theta_n(x)\,dx
=2\pi\theta_n(0)=2\pi.
$$

Consequently

$$
0\leq\int\theta_n\widehat f
=\left|\int f\widehat\theta_n\right|
\leq\|f\|_\infty\int\widehat\theta_n
=2\pi\|f\|_\infty.
$$

Passing to the limit proves

$$
\boxed{\|\widehat f\|_{L^1}\leq2\pi\|f\|_{L^\infty}.}
$$

**Thus one may take the universal constant $\alpha=2\pi$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27H](../../27h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
