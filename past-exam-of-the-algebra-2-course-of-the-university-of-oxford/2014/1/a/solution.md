<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [prime ideal](../../../../prime-ideal.md) is a proper [ideal](../../../../ideal.md) $I\neq R$ such that $ab\in I$ implies $a\in I$ or $b\in I$, for every $a,b\in R$.

Suppose first that $I$ is prime. Since $I$ is proper, $1+I\neq0+I$ in the [quotient ring](../../../../quotient-ring.md). If $(a+I)(b+I)=0+I$, then $ab\in I$, so primeness gives $a+I=0+I$ or $b+I=0+I$. Thus the commutative [quotient ring](../../../../quotient-ring.md) has a nonzero identity and no nonzero [zero divisors](../../../../zero-divisor.md), hence is an [integral domain](../../../../integral-domain.md).

Conversely, if $R/I$ is an [integral domain](../../../../integral-domain.md), its identity is nonzero, so $I\neq R$. If $ab\in I$, then $(a+I)(b+I)=0$ in $R/I$. Absence of nonzero [zero divisors](../../../../zero-divisor.md) implies $a+I=0$ or $b+I=0$, namely $a\in I$ or $b\in I$. Therefore

$$
\boxed{I\text{ is prime}\ \Longleftrightarrow\ R/I\text{ is an integral domain}.}
$$

The properness condition matters: taking $I=R$ would produce the [zero ring](../../../../zero-ring.md), which is not an [integral domain](../../../../integral-domain.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
