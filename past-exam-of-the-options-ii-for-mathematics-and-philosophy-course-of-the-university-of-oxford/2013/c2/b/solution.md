<h1 id="c2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor $a=\prod_i q_i$ and $b=\prod_j p_j$, listing prime factors with repetitions. Coprimality ensures $q_i\ne p_j$. By the definition of the [Jacobi symbol](../../../../jacobi-symbol.md) and [multiplicativity of the Legendre symbol](../../../../multiplicativity-of-the-legendre-symbol.md),

$$
(a/b)(b/a)=\prod_{i,j}(q_i/p_j)(p_j/q_i)
=(-1)^{\left(\sum_i(q_i-1)/2\right)\left(\sum_j(p_j-1)/2\right)}.
$$

For odd integers $r,s$,

$$
\frac{rs-1}{2}\equiv\frac{r-1}{2}+\frac{s-1}{2}\pmod2,
$$

since the difference is $(r-1)(s-1)/2$, an even integer. Inductively the two sums in the exponent are congruent to $(a-1)/2$ and $(b-1)/2$ modulo two. Hence

$$
\boxed{(a/b)(b/a)=(-1)^{\frac{a-1}{2}\frac{b-1}{2}}.}
$$

If either number is one, the empty product convention proves the same identity. This extends the prime law to arbitrary coprime positive odd denominators.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [C2](../../c2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Options II for mathematics and philosophy course of the University of Oxford](../../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
