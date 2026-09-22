<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the stated [Eisenstein criterion](../../../../../eisenstein-criterion.md) directly. Assume $n\geq1$. Suppose $f=gh$ in the [polynomial ring](../../../../../polynomial-ring.md) $R[X]$. Since the [principal ideal domain](../../../../../principal-ideal-domain.md) $R$ is an [integral domain](../../../../../integral-domain.md), [polynomial degree](../../../../../degree-of-a-polynomial.md) is additive under [polynomial multiplication](../../../../../polynomial-multiplication.md), and the product of the [leading coefficients](../../../../../leading-coefficient-of-a-polynomial.md) of $g,h$ is the [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $1$ of $f$. These two [coefficients](../../../../../coefficient.md) are therefore [units](../../../../../unit-in-a-ring.md). Multiplying $g$ and $h$ by inverse [units](../../../../../unit-in-a-ring.md), without changing their product, makes both factors [monic polynomials](../../../../../monic-polynomial.md).

If either factor is a [constant polynomial](../../../../../constant-polynomial.md), that factor is now $1$, so the original factor was a [unit](../../../../../unit-in-a-ring.md). It remains to rule out $r=\deg g>0$ and $s=\deg h>0$.

The [prime element](../../../../../prime-element.md) $p$ generates a [maximal ideal](../../../../../maximal-ideal.md) in the [principal ideal domain](../../../../../principal-ideal-domain.md) $R$. Indeed, if $(p)\subseteq(d)$, then $p=de$, and the [irreducible element](../../../../../irreducible-element.md) property of $p$ forces either $(d)=R$ or $(d)=(p)$. Consequently $k=R/(p)$ is a [field](../../../../../field.md). Apply [reduction modulo an ideal](../../../../../reduction-modulo-an-ideal.md) to every [coefficient](../../../../../coefficient.md). The [monic polynomial](../../../../../monic-polynomial.md) factors retain their [polynomial degrees](../../../../../degree-of-a-polynomial.md), and the hypotheses give

$$
\overline g\,\overline h=\overline f=X^n\quad\text{in }k[X].
$$

The [polynomial ring](../../../../../polynomial-ring.md) over a [field](../../../../../field.md) is a [unique factorization domain](../../../../../unique-factorization-domain.md), and $X$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md). Thus its only [monic polynomial](../../../../../monic-polynomial.md) divisors in $X^n$ are powers of $X$. Hence $\overline g=X^r$ and $\overline h=X^s$. Both have zero [constant term](../../../../../constant-term.md), so $p\mid g(0)$ and $p\mid h(0)$. This gives $p^2\mid g(0)h(0)=a_0$, a contradiction.

The [monic polynomial](../../../../../monic-polynomial.md) $f$ has positive [polynomial degree](../../../../../degree-of-a-polynomial.md), so it is a nonzero [nonunit](../../../../../nonunit.md). Every factorization therefore has a [unit](../../../../../unit-in-a-ring.md) factor, proving

$$
\boxed{f\text{ is irreducible in }R[X]}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
