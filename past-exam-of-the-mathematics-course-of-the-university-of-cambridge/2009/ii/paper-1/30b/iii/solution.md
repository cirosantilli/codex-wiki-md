<h1 id="30b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Formally the [Jacobian determinant](../../../../../../jacobian-determinant.md) of the [characteristic flow map](../../../../../../characteristic-flow-map.md) satisfies $J'=\operatorname{div}B(\Phi_t)J=0$, $J(0)=1$, so $J=1$. Changing variables $z=\Phi_t(z_0)$ gives

$$
\int_{\mathbb R^{2d}}|f(z,t)|^p\,dz=\int_{\mathbb R^{2d}}|f_I(z_0)|^p\,dz_0.
$$

Taking the $p$th root proves **$\boxed{\|f(t)\|_{L^p}=\|f_I\|_{L^p}}$** for $1\leq p<\infty$. Equivalently multiply the equation by $pf^{p-1}$ and integrate the divergence term, with vanishing boundary terms. Volume preservation gives the result without needing such boundary decay for general integrable data.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [30B](../../30b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
