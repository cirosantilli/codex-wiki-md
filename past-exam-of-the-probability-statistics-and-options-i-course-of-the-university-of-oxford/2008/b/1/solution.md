<h1 id="b/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Eisenstein's criterion](../../../../eisenstein-criterion.md) says that an integer polynomial with leading coefficient not divisible by a prime $\ell$, all other coefficients divisible by $\ell$, and constant coefficient not divisible by $\ell^2$ is irreducible over the rationals, provided it is primitive; the usual [Gauss's lemma](../../../../gauss-s-lemma-riemannian-geometry.md) supplies the passage from integer to rational factors.

Apply it with $\ell=2$ to

$$
(x+1)^8+1=x^8+8x^7+28x^6+56x^5+70x^4+56x^3+28x^2+8x+2.
$$

All nonleading coefficients are even and the constant is not divisible by four. A translation of the variable preserves reducibility, so **$x^8+1$ is irreducible over $\mathbb Q$**.

Let $\zeta=e^{i\pi/8}$ and $c=\cos(\pi/8)$. The minimal polynomial of $\zeta$ is $x^8+1$, so $[\mathbb Q(\zeta):\mathbb Q]=8$. Since $2c=\zeta+\zeta^{-1}$, the number $\zeta$ satisfies $t^2-2ct+1=0$ over $\mathbb Q(c)$. This real field cannot contain the nonreal $\zeta$, so that extension has degree exactly two. The [tower law for field extensions](../../../../tower-law-for-field-extensions.md) gives

$$
\boxed{[\mathbb Q(\zeta):\mathbb Q(c)]=2,\qquad
[\mathbb Q(c):\mathbb Q]=4.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
