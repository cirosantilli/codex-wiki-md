<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [linear regularization](../../../../../../linear-regularization.md) is a family of bounded operators $R_\alpha:Y\to X$ such that $R_\alpha y\to A^\dagger y$ for every $y$ in the domain of the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) as $\alpha\downarrow0$. For noisy data $\|y^\delta-y\|\leq\delta$, a [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md) also specifies a parameter choice $\alpha(\delta,y^\delta)$ giving convergence to $A^\dagger y$, uniformly over the allowed noise at each fixed admissible exact datum.

Expand $x_\alpha$ in the input singular vectors. The [Tikhonov normal equation](../../../../../../tikhonov-normal-equation.md) implies

$$
(\alpha+\sigma_n^2)\langle x_\alpha,u_n\rangle=\sigma_n\langle y,v_n\rangle.
$$

The component in $\ker A$ is zero because $\alpha>0$. Comparing with the given filter convention gives

$$
\boxed{f_\alpha(\sigma)=\frac{\sigma^2}{\alpha+\sigma^2},\qquad R_\alpha y=\sum_n\frac{\sigma_n}{\alpha+\sigma_n^2}\langle y,v_n\rangle u_n.}
$$

The [singular-system Tikhonov filter](../../../../../../singular-system-tikhonov-filter.md) is often described by its gain $g_\alpha(\sigma)=\sigma/(\alpha+\sigma^2)$; the requested $f_\alpha$ includes one extra factor of $\sigma$. For admissible data, $f_\alpha\to1$ and $0\leq f_\alpha\leq1$, so [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applied to the squared [Picard criterion](../../../../../../picard-criterion.md) coefficients proves exact-data convergence. Also

$$
\|R_\alpha\|\leq\sup_{\sigma\geq0}\frac{\sigma}{\alpha+\sigma^2}=\frac{1}{2\sqrt\alpha}.
$$

By the [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md), $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$ suffice for noisy-data convergence; for example $\alpha=\delta$ as $\delta\downarrow0$. This establishes both consistency and stability of [Tikhonov regularization](../../../../../../tikhonov-regularization.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
