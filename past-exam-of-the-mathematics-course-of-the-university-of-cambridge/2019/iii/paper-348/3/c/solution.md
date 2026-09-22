<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Kantorovich–Rubinstein theorem](../../../../../../kantorovich-rubinstein-theorem.md) concerns a [Polish space](../../../../../../polish-space.md) $(X,\rho)$ and [probability measures](../../../../../../probability-measure.md) $\mu,\nu$ with finite first [moments](../../../../../../moment.md), meaning $\int\rho(x,x_0)\,d\mu(x)+\int\rho(x,x_0)\,d\nu(x)<\infty$ for one, hence every, $x_0\in X$. It states

$$
\boxed{W_1(\mu,\nu)=\inf_{\pi\in\Pi(\mu,\nu)}\int\rho(x,y)\,d\pi
=\sup_{\operatorname{Lip}(f)\leq1}\left\{\int f\,d\mu-\int f\,d\nu\right\}.}
$$

Here $\operatorname{Lip}(f)\leq1$ means $|f(x)-f(y)|\leq\rho(x,y)$ for every $x,y$. The [Wasserstein distance](../../../../../../wasserstein-distance.md) with ground cost $\rho$ therefore equals a supremum over functions with [Lipschitz constant](../../../../../../lipschitz-constant.md) at most one. One may normalize $f(x_0)=0$, since adding a constant does not change the difference of integrals. This normalization bounds $|f(x)|$ by $\rho(x,x_0)$, so finite first [moments](../../../../../../moment.md) ensure integrability. The supremum is unchanged if an absolute value is placed around the difference, because $-f$ is admissible whenever $f$ is.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
