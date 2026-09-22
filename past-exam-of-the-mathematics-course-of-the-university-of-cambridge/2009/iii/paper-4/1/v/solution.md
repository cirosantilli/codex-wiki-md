<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Because $N$ is an [abelian group](../../../../../../abelian-group.md), every $\varphi\in\operatorname{Irr}(N)$ is a [linear character](../../../../../../linear-character.md), hence a homomorphism to $\mathbb C^\times$. Its [inertia group of a character](../../../../../../inertia-group-of-a-character.md) contains $N$, whose inner conjugations act trivially on $N$. Write an arbitrary $g\in G$ as $g=nh$ with $n\in N$ and $h\in H$, using $G=NH$. Conjugation by $n$ does not affect $\varphi$, so $g$ stabilizes $\varphi$ if and only if $h$ does.

Suppose $h\ne1$ stabilizes $\varphi$. Then $\varphi(h^{-1}yh)=\varphi(y)$ for every $y\in N$, and its multiplicativity gives

$$
\varphi([h,y])=\varphi(h^{-1}y^{-1}hy)=\varphi(h^{-1}yh)^{-1}\varphi(y)=1.
$$

Part (iv) makes $y\mapsto[h,y]$ surjective onto $N$, so $\varphi(x)=1$ for every $x\in N$. This would be the [trivial character](../../../../../../trivial-character.md), contrary to the hypothesis. Therefore no nonidentity $h\in H$ stabilizes $\varphi$, and

$$
\boxed{I_G(\varphi)=N\qquad(\varphi\ne1_N).}
$$

The argument uses both abelianness, to make $\varphi$ multiplicative, and the fixed-point-free commutator bijection.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
