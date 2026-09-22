<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The simpler shifted inverse is [Lavrentiev regularization](../../../../../../lavrentiev-regularization.md). Its expansion in the [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) is

$$
S_\alpha y_\delta=\sum_i\frac{(y_\delta,u_i)}{\lambda_i+\alpha}u_i.
$$

Using $y=Ax$, the exact component error is

$$
\boxed{x_\alpha^\delta-x=\sum_i\frac{e_i-\alpha x_i}{\lambda_i+\alpha}u_i,\qquad
\|x_\alpha^\delta-x\|^2=\sum_i\frac{|e_i-\alpha x_i|^2}{(\lambda_i+\alpha)^2}.}
$$

Consequently the [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md) gives

$$
\boxed{\|x_\alpha^\delta-x\|\leq\frac{\delta+\alpha\|x\|}{\lambda_1+\alpha}
\leq\frac\delta\alpha+\frac{\alpha}{\lambda_1}\|x\|.}
$$

For a prior or data-based bound $X\geq\|x\|$, [balancing noise and approximation bias](../../../../../../balancing-noise-and-approximation-bias.md) in the last expression gives

$$
\boxed{\alpha(\delta)=\sqrt{\frac{\delta\lambda_1}{X}},\qquad
\|x_{\alpha(\delta)}^\delta-x\|\leq2\sqrt{\frac{\delta X}{\lambda_1}}.}
$$

For example $X=(\|y_\delta\|+\delta)/\lambda_1$ is computable from the data and the stated noise bound. With fixed positive $\lambda_1$, $\alpha\to0$ and $\delta/\alpha\to0$ are sufficient for the robust bound to converge.

The first bound is stronger in the finite-dimensional setting. If $X>0$, choosing $\alpha=\delta/X$ gives $\|x_\alpha^\delta-x\|\leq2\delta/(\lambda_1+\delta/X)$. The unregularized inverse already has error at most $\delta/\lambda_1$; the balancing rule is a useful stabilized choice rather than a necessary cure for an unbounded inverse. A universal noise-only optimal $\alpha$ cannot be inferred without information about the size or spectral content of $x$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
