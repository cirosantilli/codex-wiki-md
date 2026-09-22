<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $f(x)=\rho(x,0)$. The first normalized [Fourier sine series](../../../../../fourier-sine-series.md) coefficient is

$$
a_1=\sqrt{\frac2L}\int_0^Lf(x)\sin\frac{\pi x}{L}\,dx>0.
$$

Strict positivity follows because $f\geq0$, has positive total mass, and $\sin(\pi x/L)>0$ everywhere inside the interval. In particular, there is no cancellation that could remove the slowest term. This is the [positivity of the first Dirichlet reaction-diffusion coefficient](../../../../../positivity-of-the-first-dirichlet-reaction-diffusion-coefficient.md).

For finite initial mass $M=\int_0^Lf(x)\,dx$, all coefficients satisfy $|a_n|\leq\sqrt{2/L}\,M$. The [eigenfunction expansion](../../../../../eigenfunction-expansion.md) therefore gives the uniform bound

$$
\left|e^{\lambda_1t}\rho(x,t)-a_1\psi_1(x)\right|\leq\frac{2M}{L}\sum_{n=2}^{\infty}e^{-D\pi^2(n^2-1)t/L^2}\longrightarrow0.
$$

The positive first profile thus controls the long-time behavior. We recover exactly the threshold $\boxed{\gamma_c=D\pi^2/L^2}$, with decay below it and unbounded positive growth at every interior point above it. The finite-mass condition is the usual meaning of an initial density profile here; standard positive-time smoothing gives the same conclusion in the usual broader admissible data classes.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
