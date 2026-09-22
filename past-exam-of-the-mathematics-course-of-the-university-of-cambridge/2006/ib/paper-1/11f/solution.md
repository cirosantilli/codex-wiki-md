<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Let $S_N(x)=\sum_{n=1}^N[a_n\cos(nx)+b_n\sin(nx)]$. Under the first coefficient bounds,

$$
\sup_{x\in\mathbb R}|S_M(x)-S_N(x)|\le2c\sum_{n>N}n^{-1-\varepsilon}\longrightarrow0.
$$

This proves the uniform Cauchy condition on the whole [real line](../../../../../real-line.md) and hence [uniform convergence](../../../../../uniform-convergence.md) to $f$. It is the [Weierstrass M-test](../../../../../weierstrass-m-test.md) applied with the summable majorant $2cn^{-1-\varepsilon}$. Every partial sum is continuous. To see continuity of the limit explicitly, at a chosen $x_0$ first choose $N$ with small uniform error; then make $|S_N(x)-S_N(x_0)|$ small by continuity. The inequality

$$
|f(x)-f(x_0)|\le|f(x)-S_N(x)|+|S_N(x)-S_N(x_0)|+|S_N(x_0)-f(x_0)|
$$

proves continuity. Also $S_N(x+2\pi)=S_N(x)$ for every $N$, so taking limits gives **$f(x+2\pi)=f(x)$**.

Under the stronger coefficient bounds, the [derivative](../../../../../derivative.md) series has summable uniform majorant $2cn^{-1-\varepsilon}$. Thus $S_N'$ converges uniformly to a continuous function $g$ given by that series. The original series also converges uniformly. On any finite interval, the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives $S_N(x)-S_N(0)=\int_0^x S_N'(t)dt$. [Uniform convergence](../../../../../uniform-convergence.md) permits passage to the limit inside this finite [integral](../../../../../integral.md), since the error is at most $|x|\|S_N'-g\|_\infty$. Therefore $f(x)-f(0)=\int_0^x g(t)dt$, and continuity of $g$ gives $f'=g$. This justifies [Termwise differentiation of a Fourier series](../../../../../termwise-differentiation-of-a-fourier-series.md) rather than assuming it:

$$
\boxed{f'(x)=-\sum_{n\ge1}na_n\sin(nx)+\sum_{n\ge1}nb_n\cos(nx).}
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
