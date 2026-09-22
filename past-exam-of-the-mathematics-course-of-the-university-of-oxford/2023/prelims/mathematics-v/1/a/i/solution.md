<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $D$ be a bounded planar region with a piecewise smooth, simple closed boundary $C$, oriented counterclockwise, and let $P,Q$ have continuous first [partial derivatives](../../../../../../../partial-derivative.md) on an open neighbourhood of its closure. [Green's theorem](../../../../../../../green-theorem.md) states that

$$
\boxed{\oint_C(P\,dx+Q\,dy)=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)dx\,dy.}
$$

For a region with holes, orient every boundary component with $D$ on its left: the outer component is counterclockwise and the inner components are clockwise.

Choose $P=-y/2$ and $Q=x/2$. Their indicated [partial derivatives](../../../../../../../partial-derivative.md) differ by one, so the [area](../../../../../../../surface-area.md) is

$$
\boxed{|D|=\iint_D1\,dx\,dy=\frac12\oint_C(x\,dy-y\,dx).}
$$

This is [signed area as a boundary integral](../../../../../../../signed-area-as-a-boundary-integral.md); reversing the direction of $C$ changes the sign of the integral.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
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
