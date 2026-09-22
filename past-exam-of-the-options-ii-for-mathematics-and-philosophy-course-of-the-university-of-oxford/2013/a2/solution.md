<h1 id="a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

A monic [quadratic polynomial](../../../quadratic-polynomial.md) over a [field](../../../field.md) is irreducible exactly when it has no root in that [field](../../../field.md). Testing the nine choices of its two coefficients in $\mathbb F_3$ gives

$$
\boxed{x^2+1,\qquad x^2+x+2,\qquad x^2+2x+2.}
$$

For clarity, a zero constant term gives a root at zero. Among constant term one, only the zero linear coefficient avoids roots at $1,2$. Among constant term two, precisely the linear coefficients one and two avoid roots. This exhausts all choices.

Put $f=x^4+x+2$. Its values at $0,1,2$ are respectively $2,1,2$, so it has no linear factor. If this quartic were reducible, absence of a linear factor would force a factorization into two irreducible quadratics. Division by the three candidates above gives remainders respectively $x,x+1,x+1$, all nonzero. Thus **$f$ is an [irreducible polynomial](../../../irreducible-polynomial.md)**.

The [quotient by an irreducible polynomial is a field](../../../quotient-by-an-irreducible-polynomial-is-a-field.md) consequently gives a [field](../../../field.md) of $3^4=81$ elements. Its nonzero elements form a [multiplicative group of a finite field](../../../multiplicative-group-of-a-finite-field.md) of order $80$. In this [field](../../../field.md), $a^4=1+2a$. Successive squaring gives

$$
a^8=1+a+a^2,\qquad a^{16}=2+a+2a^3.
$$

The latter is not one: otherwise the nonzero [polynomial](../../../polynomial-split.md) $1+x+2x^3$ of degree below four would vanish at $a$, contradicting its [minimal polynomial](../../../minimal-polynomial.md). By [Lagrange's theorem](../../../lagrange-s-theorem.md), $(a^{16})^5=a^{80}=1$. Since five is prime, its order is exactly five. Hence one answer is

$$
\boxed{\zeta=2+a+2a^3.}
$$

Its other nonidentity powers are the remaining primitive fifth roots. It is unnecessary to prove that $a$ itself generates the entire multiplicative [group](../../../group-split.md).

## ↑ Ancestors (11)

1. [A2](../a2.md)
2. [2013](../../2013-split.md)
3. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../split.md)
4. [Options II for mathematics and philosophy course of the University of Oxford](../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Mathematics and philosophy course of the University of Oxford](../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
