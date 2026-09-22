<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [group homomorphism](../../../../group-homomorphism.md) preserves multiplication, $\phi(ab)=\phi(a)\phi(b)$. A [group isomorphism](../../../../group-isomorphism.md) is a bijective homomorphism. An isomorphism from a group to itself is a [group automorphism](../../../../group-automorphism.md).

The [automorphism group](../../../../automorphism-group.md) contains the identity map. Composition is associative, and if $\phi,\psi$ are automorphisms, $(\phi\circ\psi)(ab)=\phi(\psi(a)\psi(b))=(\phi\circ\psi)(a)(\phi\circ\psi)(b)$; composition is also bijective. For $u=\phi(a)$ and $v=\phi(b)$, $\phi^{-1}(uv)=\phi^{-1}(\phi(ab))=ab=\phi^{-1}(u)\phi^{-1}(v)$, proving the inverse bijection is a homomorphism. These facts establish all group axioms.

A finite [cyclic group](../../../../cyclic-group.md) is $G=\langle g\rangle=\{e,g,\ldots,g^{n-1}\}$ with $g$ of order $n$. The map $g^k\mapsto e^{2\pi ik/n}$ is well defined modulo $n$, bijective onto the [roots of unity](../../../../root-of-unity.md), and preserves multiplication. It identifies $G$ with the multiplicative group of $n$th roots of unity.

For prime $n$, [Lagrange's theorem](../../../../lagrange-s-theorem.md) leaves only subgroup orders one and $n$: **there is no nontrivial proper subgroup**. The trivial subgroup $\{e\}$ is nevertheless proper when $n>1$, so that qualification is necessary in the printed claim. The characterization of [groups with no proper nontrivial subgroups](../../../../groups-with-no-proper-nontrivial-subgroups.md) makes the distinction explicit.

For composite $n$, choose a prime divisor $p$ and take $\boxed{H_0=\{e\},\quad H_1=\langle g^p\rangle}$, of orders $1$ and $n/p$. They are distinct proper subgroups, with $H_1$ nontrivial. If the question intended two nontrivial proper subgroups, that demand is not always possible: a cyclic group of order $p^2$ has only the one of order $p$. The [subgroups and quotients of a cyclic group](../../../../subgroups-and-quotients-of-a-cyclic-group.md) are controlled by its divisors. The order-one group is a separate trivial case, with no proper subgroups.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
