<h1 id="c/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [quadratic reciprocity](../../../../quadratic-reciprocity.md) states that for distinct odd primes $a,b$,

$$
\left(\frac ab\right)\left(\frac ba\right)
=(-1)^{(a-1)(b-1)/4}.
$$

For fixed odd prime $r$, first suppose that $p,q\ne r$. The congruence $p\equiv q\pmod{4r}$ gives the same residues modulo $r$ and modulo four. Reciprocity yields

$$
\left(\frac rp\right)
=\left(\frac pr\right)(-1)^{(r-1)(p-1)/4}
=\left(\frac qr\right)(-1)^{(r-1)(q-1)/4}
=\left(\frac rq\right).
$$

If $p=r$, the congruence forces $r\mid q$, so $q=r$ and both symbols are zero; the same handles $q=r$.

For $n=\prod_jr_j^{a_j}$, where all $r_j$ are odd primes, $4r_j$ divides $4n$. Thus $p\equiv q\pmod{4n}$ implies equality of each prime-numerator [Legendre symbol](../../../../legendre-symbol.md). Multiplicativity gives

$$
\boxed{\left(\frac np\right)
=\prod_j\left(\frac{r_j}p\right)^{a_j}
=\prod_j\left(\frac{r_j}q\right)^{a_j}
=\left(\frac nq\right).}
$$

This also covers symbols that vanish; for $n=1$ both sides are one.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [C](../../c.md)
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
