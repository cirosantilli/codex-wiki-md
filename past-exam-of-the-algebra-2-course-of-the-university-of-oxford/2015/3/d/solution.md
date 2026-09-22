<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $I=(2,t)\subseteq\mathbb Z[t]$. The [ring homomorphism](../../../../ring-homomorphism.md)

$$
\theta:\mathbb Z[t]\longrightarrow\mathbb F_2,
\qquad \theta(g)=g(0)\pmod2
$$

is surjective. Its [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) is exactly $I$: a [polynomial](../../../../polynomial-split.md) maps to zero precisely when its constant coefficient is even, in which case it has the form $2a+th(t)$ with $a\in\mathbb Z$ and $h\in\mathbb Z[t]$. By the [first isomorphism theorem for rings](../../../../first-isomorphism-theorem-for-rings.md),

$$
\mathbb Z[t]/I\cong\mathbb F_2.
$$

This [quotient ring](../../../../quotient-ring.md) is a [field](../../../../field.md), so $I$ is a [maximal ideal](../../../../maximal-ideal.md) and in particular a [prime ideal](../../../../prime-ideal.md).

Suppose $I=(h)$ were a [principal ideal](../../../../principal-ideal.md). Because $2\in I$, the nonzero [polynomial](../../../../polynomial-split.md) $h$ divides the constant $2$, forcing its [polynomial degree](../../../../degree-of-a-polynomial.md) to be zero: $h=d$ for a nonzero [integer](../../../../integer-split.md) $d$. But $t\in I$ also makes $d$ divide the coefficient $1$ of $t$, so $d=\pm1$. This would give $I=\mathbb Z[t]$, contradicting the properness of the [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) $\ker\theta$. Therefore

$$
\boxed{(2,t)\text{ is a prime ideal of }\mathbb Z[t]
\text{ that is not principal}.}
$$

There is no conflict with part (c): $I\cap\mathbb Z=2\mathbb Z\ne\{0\}$. The zero-intersection hypothesis is exactly what excludes this example.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
