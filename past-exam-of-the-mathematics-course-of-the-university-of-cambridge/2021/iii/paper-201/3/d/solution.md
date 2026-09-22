<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
T=\inf\{k\leq n:S_k-\mu k\geq\varepsilon n\}\wedge n.
$$

On $A$, one has $T\leq n$, $S_T\geq\mu T+\varepsilon n$, and convexity of $\psi$ gives $\psi(\theta)-\mu\theta\geq0$. Hence for $\theta>0$,

$$
Z_T
=e^{\theta(S_T-\mu T)-(\psi(\theta)-\mu\theta)T}
\geq e^{(\theta(\mu+\varepsilon)-\psi(\theta))n}.
$$

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applies because $T$ is bounded, so $\mathbb EZ_T=1$. Therefore

$$
\boxed{\mathbb P(A)\leq e^{-(\theta(\mu+\varepsilon)-\psi(\theta))n}}.
$$

Optimize over $\theta>0$ for the upper deviation and apply the same argument with $\theta<0$ to the lower deviation. Since the supremum of the linearly interpolated centered walk is attained at grid points, the [Legendre transform of a cumulant-generating function](../../../../../../legendre-transform-of-a-cumulant-generating-function.md)

$$
\psi^*(x)=\sup_{\theta\in\mathbb R}(\theta x-\psi(\theta))
$$

and the [union bound](../../../../../../boole-s-inequality.md) give

$$
\boxed{
\mathbb P\left(\sup_{0\leq t\leq1}|S_t^{(n)}-\mu t|\geq\varepsilon\right)
\leq e^{-n\psi^*(\mu+\varepsilon)}+e^{-n\psi^*(\mu-\varepsilon)}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
