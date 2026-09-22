<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A covariant derivative is an $\mathbb R$-linear map

$$
d_A:\Gamma(E)\to\Omega^1(B;E)
$$

satisfying $d_A(fs)=df\otimes s+f\,d_As$. It is local: its value over an open set depends only on the restriction of the section there. A horizontal connection differentiates a section, projects its derivative vertically, and identifies the vertical tangent with the fibre.

In a local frame write $d_As=ds+A_is\,dy^i$. If $x^a$ are coordinates on $M$, the defining identity in the question forces

$$
d_{A'}(s\circ f)=d(s\circ f)+A'_a(s\circ f)\,dx^a
$$

with

$$
\boxed{A'_a(x)=A_i(f(x))\frac{\partial f^i}{\partial x^a}(x).}
$$

**Thus $A'=f^*A$, the [pullback connection](../../../../../../pullback-connection.md).**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
