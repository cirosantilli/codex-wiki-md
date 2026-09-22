<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [partial derivatives](../../../../../../partial-derivative.md) of this [parametrized surface](../../../../../../parametrized-surface.md) are

$$
\mathbf r_s=(t\cos t,t\sin t,2),\qquad
\mathbf r_t=s(\cos t-t\sin t,\sin t+t\cos t,0).
$$

Their [cross product](../../../../../../cross-product.md) is

$$
\mathbf r_s\times\mathbf r_t
=s\bigl(-2(\sin t+t\cos t),\ 2(\cos t-t\sin t),\ t^2\bigr).
$$

The mixed terms cancel in its squared [Euclidean norm](../../../../../../euclidean-norm.md):

$$
|\mathbf r_s\times\mathbf r_t|^2
=s^2\bigl(4(1+t^2)+t^4\bigr)=s^2(t^2+2)^2.
$$

Since $s>0$, the [surface area element](../../../../../../surface-area-element.md) is $s(t^2+2)\,ds\,dt$. There is no repeated coverage: $z=2s$ recovers $s$, and $\sqrt{x^2+y^2}=st$ then recovers $t$. Therefore the [surface area](../../../../../../surface-area.md) is

$$
\begin{aligned}
\operatorname{area}(S)
&=\int_0^{2\pi}\int_0^1s(t^2+2)\,ds\,dt\\
&=\frac12\left[\frac{t^3}{3}+2t\right]_0^{2\pi}
=\boxed{\frac{4\pi^3}{3}+2\pi}.
\end{aligned}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
