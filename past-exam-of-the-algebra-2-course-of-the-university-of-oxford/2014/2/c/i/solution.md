<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the reduction criterion: a primitive integer-coefficient [polynomial](../../../../../polynomial-split.md) whose leading coefficient remains nonzero modulo a [prime number](../../../../../prime-number-split.md) $p$ is irreducible over $\mathbb Q$ if its reduction is irreducible over $\mathbb F_p$. This follows from [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md), since a nontrivial factorization over the integers would reduce to a nontrivial factorization of the same degrees. For a monic polynomial the factors may be taken monic, so neither degree can drop.

Modulo $2$ the polynomial is $\overline f=t^4+t+1$. Its values at $0$ and $1$ are both $1$, so it has no [linear polynomial](../../../../../linear-polynomial.md) factor. A reducible [quartic polynomial](../../../../../quartic-polynomial.md) without a [linear polynomial](../../../../../linear-polynomial.md) factor must factor into two irreducible [quadratic polynomials](../../../../../quadratic-polynomial.md). The only monic irreducible [quadratic polynomial](../../../../../quadratic-polynomial.md) over $\mathbb F_2$ is $q=t^2+t+1$: among monic [quadratic polynomials](../../../../../quadratic-polynomial.md) a nonzero constant is necessary, and $t^2+1$ has a root, while $q$ has none.

But $t^2\equiv t+1\pmod q$, so $t^3\equiv1$ and $t^4\equiv t$. Consequently

$$
\overline f\equiv t+t+1=1\pmod q.
$$

Thus $q$ does not divide $\overline f$, excluding the remaining possible factorization. We obtain

$$
\boxed{t^4+t+1\text{ is irreducible over }\mathbb Q.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 2 course of the University of Oxford](../../../../split.md)
6. [Algebra 2 course of the University of Oxford](../../../../../algebra-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
