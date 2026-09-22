<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a finite graph $\Lambda=(V,E)$ with [free boundary conditions](../../../../../../free-boundary-condition.md), write $\sigma_x=(\cos\theta_x,\sin\theta_x)\in S^1$. The ferromagnetic [O(2) model](../../../../../../xy-model.md) is

$$
d\mu_{\Lambda,\beta,h}(\theta)
=\frac1Z\exp\left\{\beta\sum_{xy\in E}\cos(\theta_x-\theta_y)
+h\sum_{x\in V}\cos\theta_x\right\}
\prod_{x\in V}\frac{d\theta_x}{2\pi}.
$$

The [Ginibre inequality](../../../../../../ginibre-inequality.md) says, in particular, that for $a,b\in\mathbb Z_{\geq0}^V$,

$$
\langle\cos(a\cdot\theta)\cos(b\cdot\theta)\rangle
\geq
\langle\cos(a\cdot\theta)\rangle
\langle\cos(b\cdot\theta)\rangle.
$$

For the proof, take two independent replicas $\theta,\theta'$ and write the covariance as one half of the expectation of

$$
\{\cos(a\cdot\theta)-\cos(a\cdot\theta')\}
\{\cos(b\cdot\theta)-\cos(b\cdot\theta')\}.
$$

Set $u=(\theta+\theta')/2$ and $v=(\theta-\theta')/2$. Product-to-sum identities turn each difference into $-2\sin(a\cdot u)\sin(a\cdot v)$, while every replicated interaction becomes

$$
\cos(\theta_x-\theta_y)+\cos(\theta'_x-\theta'_y)
=2\cos(u_x-u_y)\cos(v_x-v_y).
$$

Expand every exponential in a power series and then every cosine power into Fourier modes. Integration over each angle kills all unmatched modes. Because the couplings, field, and entries of $a,b$ are nonnegative, every surviving paired coefficient in the covariance is nonnegative. Their sum is therefore nonnegative, proving the inequality. The same replica expansion proves the usual product version.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
