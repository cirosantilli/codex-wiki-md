<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Perform the product and inverse formulas from part (b) in the commutative ring $\mathbb Z/4\mathbb Z$. They involve only addition, multiplication and negatives, so closure and inverses remain valid; no division by a nonunit is needed. Associativity again comes from matrix multiplication, and $A(0,0,0)$ remains the identity. The [Heisenberg group over a commutative ring](../../../../../heisenberg-group-over-a-commutative-ring.md) therefore has

$$
\boxed{|G|=4^3=64.}
$$

These are residues modulo four, not arithmetic in the [finite field](../../../../../finite-field.md) of four elements.

For the additional subgroup task, write an element of $H$ as $A(t,y,t)$. Its product and inverse are

$$
A(t,y,t)A(s,v,s)=A(t+s,y+v+ts,t+s),\qquad A(t,y,t)^{-1}=A(-t,t^2-y,-t).
$$

Both remain in $H$, and the product is unchanged on exchanging the factors because $ts=st$. The identity is included, so $H$ is an [Abelian subgroup](../../../../../abelian-subgroup.md). There are four independent choices each for $t,y$, giving

$$
\boxed{|H|=16,\qquad[G:H]=\frac{64}{16}=4.}
$$

Thus there are four distinct left [cosets](../../../../../coset.md). Explicitly the surjective [group homomorphism](../../../../../group-homomorphism.md) $A(x,y,z)\mapsto x-z\pmod4$ has kernel $H$; the four cosets are the level sets of that difference, with representatives $A(d,0,0)$, $d=0,1,2,3$. This is the [Abelian plane subgroup of the Heisenberg group modulo four](../../../../../abelian-plane-subgroup-of-the-heisenberg-group-modulo-four.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
