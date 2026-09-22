<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The displayed [vector field](../../../../../../../vector-field.md) is defined on the punctured plane $U=\mathbb R^2\setminus\{(0,0)\}$; it is undefined at the origin. Take the counterclockwise unit [circle](../../../../../../../circle.md) $\mathbf r(t)=(\cos t,\sin t)$, $0\leq t\leq2\pi$. Along it,

$$
\mathbf F(\mathbf r(t))=(-\sin t,\cos t)=\mathbf r'(t),\qquad
\boxed{\oint_C\mathbf F\cdot d\mathbf r=\int_0^{2\pi}1\,dt=2\pi.}
$$

By the [fundamental theorem for line integrals](../../../../../../../fundamental-theorem-for-line-integrals.md), it has no single-valued [potential of a conservative vector field](../../../../../../../potential-of-a-conservative-vector-field.md) on $U$. In particular it cannot be the restriction of the [gradient](../../../../../../../gradient.md) of a [smooth function](../../../../../../../smooth-function.md) on all of $\mathbb R^2$.

For $(x,y)\ne(0,0)$, direct differentiation gives

$$
\frac{\partial Q}{\partial x}
=\frac{x^2+y^2-2x^2}{(x^2+y^2)^2}
=\frac{y^2-x^2}{(x^2+y^2)^2}
=\frac{\partial P}{\partial y}.
$$

There is no contradiction with [Green's theorem](../../../../../../../green-theorem.md): $\mathbf F$ is not defined, let alone continuously differentiable, throughout the disk enclosed by $C$. On an annulus the theorem does apply; the counterclockwise outer integral is $2\pi$, and the clockwise inner integral is $-2\pi$, so their sum is zero. The hole prevents this [curl-free vector field](../../../../../../../irrotational-vector-field.md) from being a [conservative vector field](../../../../../../../conservative-vector-field.md) on its entire domain.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
