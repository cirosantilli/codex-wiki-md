<h1 id="b/b1/solution">Solution</h1>

↑ **Parent:** [B1](../b1.md)

[Eisenstein criterion](../../../../eisenstein-criterion.md) says that a primitive [integer](../../../../integer-split.md) [polynomial](../../../../polynomial-split.md) is irreducible over $\mathbb Q$ if some prime divides all coefficients except the leading one, does not divide the leading coefficient, and its square does not divide the constant coefficient. The passage from primitive [integer](../../../../integer-split.md) factorization to rational factorization is [Gauss lemma for polynomials](../../../../gauss-lemma-for-polynomials.md).

Translate the variable:

$$
(x+1)^8+1=x^8+8x^7+28x^6+56x^5+70x^4+56x^3+28x^2+8x+2.
$$

This is Eisenstein at two. Translation is an automorphism of $\mathbb Q[x]$, so $x^8+1$ itself is irreducible.

Set $\zeta=e^{i\pi/8}$ and $c=\cos(\pi/8)$. Since $\zeta$ is a root of that irreducible degree-eight [polynomial](../../../../polynomial-split.md), $[\mathbb Q(\zeta):\mathbb Q]=8$. Also $c=(\zeta+\zeta^{-1})/2$, so $\mathbb Q(c)\subseteq\mathbb Q(\zeta)$ and $\zeta$ solves $T^2-2cT+1=0$. The extension degree is at most two. It is not one, since every element of $\mathbb Q(c)$ is real and $\zeta$ is not. The [tower law for field extensions](../../../../tower-law-for-field-extensions.md) now gives

$$
\boxed{[\mathbb Q(\zeta):\mathbb Q(c)]=2,\qquad[\mathbb Q(c):\mathbb Q]=4}.
$$

## ↑ Ancestors (12)

1. [B1](../b1.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
