<h1 id="c/c1/solution">Solution</h1>

↑ **Parent:** [C1](../c1.md)

The [quadratic reciprocity law](../../../../quadratic-reciprocity.md) states that distinct odd primes $a,b$ satisfy

$$
\left(\frac ab\right)\left(\frac ba\right)=(-1)^{((a-1)/2)((b-1)/2)}.
$$

First suppose $p\ne q$. If the odd prime $r$ equalled one of them, divisibility of $p-q$ by $r$ would force the other to equal $r$ too, a contradiction. Thus reciprocity applies to $r,p$ and $r,q$. The [modular congruence](../../../../modular-congruence.md) modulo $4r$ gives both $p\equiv q\pmod r$ and $p\equiv q\pmod4$. Therefore $(p/r)=(q/r)$, and the reciprocity signs are identical. Rearranging the two reciprocity identities proves $\boxed{(r/p)=(r/q)}$. If $p=q$, the equality is immediate, including a zero [Legendre symbol](../../../../legendre-symbol.md) when $p=r$.

For general odd $n>1$, factor $n=\prod_jr_j^{e_j}$. If $p=q$ there is nothing to prove. Otherwise neither $p$ nor $q$ divides $n$, since any such divisor, together with $4n\mid p-q$, would force $p=q$. Each $4r_j$ divides $p-q$, so the first result and multiplicativity of the [Legendre symbol](../../../../legendre-symbol.md) give

$$
\left(\frac np\right)=\prod_j\left(\frac{r_j}p\right)^{e_j}
=\prod_j\left(\frac{r_j}q\right)^{e_j}
=\boxed{\left(\frac nq\right)}.
$$

For $n=1$, both symbols equal one.

## ↑ Ancestors (12)

1. [C1](../c1.md)
2. [C](../../c.md)
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
