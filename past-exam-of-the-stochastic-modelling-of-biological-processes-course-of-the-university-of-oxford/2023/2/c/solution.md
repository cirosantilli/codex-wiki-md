<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a radial function $f(r)$ in three dimensions, the [Laplacian](../../../../laplacian.md) is $f''+2f'/r$, while the imposed radial [drift](../../../../drift-coefficient.md) contributes $-\alpha f'/r$. Thus the radial [generator of an SDE diffusion](../../../../generator-of-an-sde-diffusion.md) is

$$
L_rf=f''+\frac{2-\alpha}{r}f'.
$$

The [hitting probability](../../../../hitting-probability.md) for the inner [sphere](../../../../sphere.md) is [harmonic](../../../../harmonic-function.md) for this [diffusion generator](../../../../diffusion-generator.md) in the shell, with value one on the inner [sphere](../../../../sphere.md) and zero on the outer [sphere](../../../../sphere.md). At $\alpha=1$, the [boundary value problem](../../../../boundary-value-problem-split.md) is therefore

$$
p''(r)+\frac1rp'(r)=0,
\qquad p(R_1)=1,\qquad p(R_2)=0.
$$

Integrating $(rp')'=0$ gives $p(r)=A\log r+B$. The two [boundary conditions](../../../../boundary-condition.md) determine

$$
\boxed{p(r_0)=\frac{\log(R_2/r_0)}{\log(R_2/R_1)}.}
$$

Both arguments of the [logarithms](../../../../logarithm.md) are dimensionless. The result decreases from one to zero across the shell and lies strictly between zero and one for $R_1<r_0<R_2$.

For a direct [probability](../../../../probability.md) interpretation, stop at the first contact $T$ with either [sphere](../../../../sphere.md). The stopped process $p(r(t\wedge T))$ is a bounded [martingale](../../../../martingale-split.md) by [Itô's formula](../../../../ito-s-lemma.md). The shell has positive inner [radius](../../../../radius.md), so its [drift](../../../../drift-coefficient.md) is bounded and its [diffusion](../../../../diffusion.md) is nondegenerate; exit occurs almost surely. [Optional stopping](../../../../optional-sampling-theorem-for-a-supermartingale.md) and [dominated convergence](../../../../dominated-convergence-theorem.md) therefore give

$$
p(r_0)=\mathbb E p(r(T))=\mathbb P\bigl(r(T)=R_1\bigr).
$$

The [logarithm](../../../../logarithm.md) appears because the inward [drift](../../../../drift-coefficient.md) cancels one of the two geometric $f'/r$ terms in the three-dimensional radial [Laplacian](../../../../laplacian.md), leaving the same radial [diffusion generator](../../../../diffusion-generator.md) as a planar [Brownian motion](../../../../brownian-motion-split.md) with [diffusion coefficient](../../../../diffusion-coefficient.md) one.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
