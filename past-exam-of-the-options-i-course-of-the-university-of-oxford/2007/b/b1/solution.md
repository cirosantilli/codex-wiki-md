<h1 id="b/b1/solution">Solution</h1>

↑ **Parent:** [B1](../b1.md)

The degree $[K:F]$ is the dimension of $K$ as a vector space over $F$. The tower theorem states that for intermediate fields $F\subseteq E\subseteq K$ in a finite extension,

$$
[K:F]=[K:E][E:F].
$$

If the degree is prime, one factor must be one, forcing $E=K$ or $E=F$; no strictly intermediate field exists.

Let $K$ have 32 elements. Its prime subfield is $\mathbb F_2$ and $[K:\mathbb F_2]=5$. Every element outside that subfield has [minimal polynomial](../../../../minimal-polynomial.md) of degree five, by the tower theorem. Also every member of $K$ satisfies $x^{32}=x$: nonzero elements form a [group](../../../../group-split.md) of order 31. Hence $x^{32}-x$ splits over $K$, with distinct roots because its derivative is $-1=1$ in characteristic two.

Every irreducible degree-five polynomial over $\mathbb F_2$ divides $x^{32}-x$. Indeed its quotient field has 32 elements, and its [residue](../../../../residue.md) class of $x$ satisfies that equation. Thus every such polynomial splits into five distinct roots in $K$. Conversely each of the 30 elements outside $\mathbb F_2$ has one such [minimal polynomial](../../../../minimal-polynomial.md), and different minimal polynomials have disjoint root sets. Consequently the number is

$$
\boxed{30/5=6}.
$$

There is no extra leading-coefficient factor, since every nonzero leading coefficient over $\mathbb F_2$ is one.

## ↑ Ancestors (12)

1. [B1](../b1.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
