<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

The [partial derivatives](../../../../../../../partial-derivative.md) of the [parametrization](../../../../../../../parametric-equation.md) are

$$
\begin{aligned}
\mathbf r_\theta&=(-\sin\theta/\sqrt2,\cos\theta\cos\phi,\cos\theta\sin\phi),\\
\mathbf r_\phi&=(0,-\sin\theta\sin\phi,\sin\theta\cos\phi).
\end{aligned}
$$

Their [cross product](../../../../../../../cross-product.md) is

$$
\mathbf r_\theta\wedge\mathbf r_\phi
=\left(\sin\theta\cos\theta,\frac{\sin^2\theta\cos\phi}{\sqrt2},\frac{\sin^2\theta\sin\phi}{\sqrt2}\right).
$$

Taking its [euclidean norm](../../../../../../../euclidean-norm.md) gives the [surface area element](../../../../../../../surface-area-element.md)

$$
dA=\frac{\sin\theta}{\sqrt2}\sqrt{1+\cos^2\theta}\,d\theta\,d\phi.
$$

The two poles and duplicated seam have zero [surface area](../../../../../../../surface-area.md), so integrating over the stated [parameter domain](../../../../../../../parameter-domain.md) counts the [surface area](../../../../../../../surface-area.md) once. With the [change of variables](../../../../../../../change-of-variables-formula.md) $u=\cos\theta$ and the supplied [definite integral](../../../../../../../definite-integral.md),

$$
\begin{aligned}
\operatorname{area}(S)
&=\frac{2\pi}{\sqrt2}\int_0^\pi\sin\theta\sqrt{1+\cos^2\theta}\,d\theta\\
&=\sqrt2\pi\int_{-1}^1\sqrt{1+u^2}\,du\\
&=\boxed{2\pi+\sqrt2\pi\ln(1+\sqrt2).}
\end{aligned}
$$

Here $-\ln(\sqrt2-1)=\ln(\sqrt2+1)$ because $(\sqrt2-1)(\sqrt2+1)=1$.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [3](../../../3.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
