<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write a rational [root of a polynomial](../../../../root-of-a-polynomial.md) as $\gamma=a/b$ in lowest terms with $b>0$. Substituting into the monic integer-coefficient [polynomial](../../../../polynomial-split.md) and multiplying by $b^d$ gives

$$
a^d+c_{d-1}a^{d-1}b+c_{d-2}a^{d-2}b^2+\cdots+c_0b^d=0.
$$

Every term other than $a^d$ is divisible by $b$, so $b\mid a^d$. But $\gcd(a,b)=1$ implies $\gcd(a^d,b)=1$, and hence $b=1$. Thus

$$
\boxed{\gamma\in\mathbb Z.}
$$

This is the monic case of the [rational root theorem](../../../../rational-root-theorem.md). The [monic polynomial](../../../../monic-polynomial.md) assumption is essential because it removes any leading coefficient that could supply prime factors of the denominator.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
