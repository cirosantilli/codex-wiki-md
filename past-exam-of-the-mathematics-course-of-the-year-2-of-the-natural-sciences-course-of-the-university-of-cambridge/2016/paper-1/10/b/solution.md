<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the intended [infinite square well](../../../../../infinite-square-well.md) interpretation: the kinetic-energy operator on $(-a,a)$ with zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). The variational [energy](../../../../../energy-split.md) is most safely evaluated through its [quadratic form](../../../../../quadratic-form-split.md),

$$
F[\phi]=\frac{\hbar^2}{2m}\frac{\int_{-a}^a|\phi'(x)|^2\,dx}{\int_{-a}^a|\phi(x)|^2\,dx}.
$$

The boundary term vanishes because the trial function vanishes at both walls. Its zero extension has [derivative](../../../../../derivative.md) jumps there, so the form interpretation avoids assigning an unrestricted full-line second [derivative](../../../../../derivative.md) to it.

Set $u=x/a$ and $b=\lambda a^2$. Apart from an irrelevant factor $a^2$, the trial function is $q_b(u)=(1-u^2)(1+bu^2)$. [Polynomial](../../../../../polynomial-split.md) [integration](../../../../../integral-split.md) gives

$$
\begin{aligned}
D(b)&=\int_{-1}^1q_b^2\,du=\frac{16}{315}(b^2+6b+21),\\
N(b)&=\int_{-1}^1(q_b')^2\,du=\frac8{105}(11b^2+14b+35).
\end{aligned}
$$

Hence the [polynomial Rayleigh-Ritz trial space for a one-dimensional box](../../../../../polynomial-rayleigh-ritz-trial-space-for-a-one-dimensional-box.md) has [energy](../../../../../energy-split.md)

$$
F(b)=\frac{\hbar^2}{ma^2}\frac{3(11b^2+14b+35)}{4(b^2+6b+21)}.
$$

The denominator is strictly positive, since $b^2+6b+21=(b+3)^2+12$. Differentiation gives

$$
\frac{ma^2}{\hbar^2}\frac{dF}{db}=\frac{3(13b^2+98b+21)}{(b^2+6b+21)^2}.
$$

The two stationary parameters are $b_\pm=(-49\pm4\sqrt{133})/13$. The smaller is a local maximum; the larger is a local minimum. Since the [energy](../../../../../energy-split.md) tends to $33\hbar^2/(4ma^2)$ as $|b|\to\infty$, the latter is the global minimum:

$$
\boxed{\lambda_* =\frac{-49+4\sqrt{133}}{13a^2}\simeq-\frac{0.220750}{a^2},\qquad E_{\rm upper}=\left(7-\frac{\sqrt{133}}2\right)\frac{\hbar^2}{ma^2}\simeq1.233718703\frac{\hbar^2}{ma^2}.}
$$

The upper stationary value is $(7+\sqrt{133}/2)\hbar^2/(ma^2)$. Exact roots give a slightly tighter bound than substituting the rounded hints.

**There are two qualifications to the printed operator and comparison [energy](../../../../../energy-split.md).** For the box with [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and width $2a$, the actual [ground-state energy](../../../../../ground-state-energy.md) is

$$
\boxed{E_0^{\rm box}=\frac{\pi^2\hbar^2}{8ma^2}\simeq1.233700550\frac{\hbar^2}{ma^2},}
$$

which lies just below the variational result. The coefficient $6/5$ printed as an exact [eigenvalue](../../../../../eigenvalue.md) is inconsistent with this box problem. Also, merely declaring the differential expression to be zero outside the interval does not impose hard-wall confinement or specify a self-adjoint domain. Read literally on a space admitting exterior-supported states, it has zero-energy states outside and does not have the claimed positive ground [energy](../../../../../energy-split.md). The boxed variational result is the well-defined answer for the intended confined particle; a different full-line operator would need its domain and matching conditions supplied.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
