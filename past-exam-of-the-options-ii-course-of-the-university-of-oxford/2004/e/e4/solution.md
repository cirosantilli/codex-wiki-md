<h1 id="e/e4/solution">Solution</h1>

↑ **Parent:** [E4](../e4.md)

For the [quotient map](../../../../quotient-map.md) $\pi$, a subset $U$ of the quotient is open exactly when $\pi^{-1}(U)$ is open in $X$. This definition immediately makes $\pi$ continuous. If $g$ is continuous then $g\circ\pi$ is continuous. Conversely, [continuity](../../../../continuous-function.md) of the composition gives, for every open $V\subseteq Z$, that $\pi^{-1}(g^{-1}(V))$ is open. By the defining criterion $g^{-1}(V)$ is open, so $g$ is continuous.

A map $h$ constant on each [equivalence class](../../../../equivalence-class.md) defines a unique map $\bar h([x])=h(x)$. It is well-defined by the assumed class constancy, and its composition with $\pi$ is $h$. The preceding criterion proves that $\bar h$ is continuous.

For the integer [lattice](../../../../lattice.md) quotient, define

$$
F(x,y)=(e^{2\pi ix},e^{2\pi iy}).
$$

This continuous map is onto the product of the two unit circles, and its fibres are exactly the [lattice](../../../../lattice.md) equivalence classes. It therefore induces a [continuous bijection](../../../../continuous-bijection.md) $\bar F:\mathbb R^2/\mathbb Z^2\to\mathbb T^2$. Every class has a representative in $[0,1]^2$, so the quotient is the continuous image of that [compact](../../../../compact-space.md) square and is [compact](../../../../compact-space.md). The target is [Hausdorff](../../../../hausdorff-space.md) as a subspace of $\mathbb C^2$. A [continuous bijection](../../../../continuous-bijection.md) from a [compact](../../../../compact-space.md) space to a [Hausdorff](../../../../hausdorff-space.md) space is a [homeomorphism](../../../../homeomorphism.md), proving

$$
\boxed{\mathbb R^2/\mathbb Z^2\cong\mathbb T^2.}
$$

Finally, if $U\subseteq\mathbb R^2$ is open, then $\pi^{-1}(\pi(U))=\bigcup_{m\in\mathbb Z^2}(U+m)$ is open, being a union of translates. The quotient criterion makes $\pi(U)$ open. Thus **the [quotient map](../../../../quotient-map.md) is an [open map](../../../../open-map.md)**.

## ↑ Ancestors (12)

1. [E4](../e4.md)
2. [E](../../e.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
