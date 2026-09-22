<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [stochastic differential equation](../../../../stochastic-differential-equation.md) $dX_s=b(s,X_s)\,ds+\Sigma(s,X_s)\,dB_s$, the [diffusion generator](../../../../diffusion-generator.md) on smooth functions is

$$
(\mathcal L_sg)(x)=\sum_jb_j(s,x)\partial_jg(x)
+\frac12\sum_{j,k}(\Sigma\Sigma^{\mathsf T})_{jk}(s,x)\partial_{jk}g(x).
$$

One form of the [Feynman-Kac formula](../../../../feynman-kac-formula.md) is the following. Suppose the [stochastic differential equation](../../../../stochastic-differential-equation.md) is well posed and nonexplosive, $c\geq0$ is bounded, the terminal data $g$ and source $h$ are bounded, and $F$ is a [classical solution](../../../../classical-solution.md) bounded on finite time intervals of

$$
\partial_tF+\mathcal L_tF-cF+h=0,\qquad F(T,x)=g(x).
$$

With the regularity needed for the [Itô formula](../../../../ito-s-lemma.md), the [parabolic Feynman-Kac formula with a source](../../../../parabolic-feynman-kac-formula-with-a-source.md) states

$$
\boxed{\begin{aligned}
F(t,x)=\mathbb E_{t,x}\bigg[&e^{-\int_t^Tc(r,X_r)\,dr}g(X_T)\\
&+\int_t^Te^{-\int_t^sc(r,X_r)\,dr}h(s,X_s)\,ds\bigg].
\end{aligned}}
$$

Here $\mathbb E_{t,x}$ means expectation for the [diffusion process](../../../../markov-diffusion.md) started at $X_t=x$. Under hypotheses ensuring existence of a [classical solution](../../../../classical-solution.md), this representation also identifies that solution uniquely in the stated bounded class. In the remaining parts, $c=h=0$, so $F(t,x)=\mathbb E_{t,x}g(X_T)$ solves the terminal-value [Kolmogorov backward equation](../../../../kolmogorov-backward-equation.md) $F_t+\mathcal L_tF=0$. Complex terminal data are allowed by applying the real formula to their [real part](../../../../real-part.md) and [imaginary part](../../../../imaginary-part.md) separately.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
