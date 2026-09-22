<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [group homomorphism](../../../../group-homomorphism.md) preserves multiplication: $\Phi(gh)=\Phi(g)\Phi(h)$. Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) $K=\{g:\Phi(g)=e_H\}$ is a subgroup, and $\Phi(gkg^{-1})=e_H$ for $k\in K$. Thus $gKg^{-1}=K$, proving it is a [normal subgroup](../../../../normal-subgroup.md). The map $gK\mapsto\Phi(g)$ is well-defined because two representatives of a coset differ by an element of $K$. It is a homomorphism, has trivial kernel, and is surjective when $\Phi$ is. This proves the [first isomorphism theorem](../../../../first-isomorphism-theorem.md), $G/K\cong H$. This proof does not use finiteness and therefore also applies below.

The identity [matrix](../../../../matrix.md) belongs to $SL_2(\mathbb C)$. The [determinant](../../../../determinant.md) is multiplicative, giving closure, and [matrix](../../../../matrix.md) multiplication is associative. The inverse of a determinant-one [matrix](../../../../matrix.md) $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ is $\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$, also of determinant one. Thus this [special linear group](../../../../special-linear-group.md) is a group.

The fractional linear maps must be interpreted on the [Riemann sphere](../../../../riemann-sphere.md), including infinity: a finite pole is sent to infinity and infinity is sent to $a/c$ when $c\ne0$. As literal everywhere-defined maps of the complex plane they would not form the asserted group. Substitution into the two rational expressions gives $f_A\circ f_B=f_{AB}$. Matrix identities and inverses therefore give the identity and inverse transformations, proving that the [Möbius group](../../../../mobius-group.md) is a group and that $\Phi:A\mapsto f_A$ is a surjective homomorphism.

For $f_A$ to be the identity, $(az+b)/(cz+d)=z$ on all finite points where defined. Hence $cz^2+(d-a)z-b$ is the zero polynomial, so $b=c=0$, $d=a$, and $a^2=1$ from the determinant. Therefore

$$
\boxed{\ker\Phi=\{I,-I\},\qquad\mathcal M\cong SL_2(\mathbb C)/\{\pm I\}=PSL_2(\mathbb C).}
$$

The kernel is central and hence normal. In particular $\Phi$ is **not an [isomorphism](../../../../isomorphism.md)**, since $A$ and $-A$ represent the same transformation. The quotient is the [projective special linear group](../../../../projective-special-linear-group.md) in this complex two-dimensional case.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
