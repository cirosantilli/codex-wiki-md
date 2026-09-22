<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Euclidean domain](../../../../euclidean-domain.md) is an [integral domain](../../../../integral-domain.md) $R$ with a [Euclidean function](../../../../euclidean-function.md) $\nu:R\setminus\{0\}\to\mathbb Z_{\geq0}$ such that, for $a,b\in R$ with $b\ne0$, there exist $q,r\in R$ satisfying

$$
a=qb+r,\qquad r=0\ \text{or}\ \nu(r)<\nu(b).
$$

The [polynomial ring](../../../../polynomial-ring.md) $\mathbb Q[x]$ has this property with $\nu(f)=\deg f$. To perform [polynomial division](../../../../polynomial-division.md), subtract an appropriate multiple of the divisor to cancel the leading term of the current remainder. Its [polynomial degree](../../../../degree-of-a-polynomial.md) decreases strictly at each step, so the process terminates below the divisor's degree. The required division of leading coefficients is possible in the [field](../../../../field.md) $\mathbb Q$. Thus a [polynomial ring over a field is Euclidean](../../../../polynomial-ring-over-a-field-is-euclidean.md), with the same argument applying to every field.

Now let $I$ be a nonzero [ideal](../../../../ideal.md) of a [Euclidean domain](../../../../euclidean-domain.md), and choose $b\in I\setminus\{0\}$ with the least possible value of $\nu(b)$. For every $a\in I$, divide $a=qb+r$. The remainder belongs to $I$, since $r=a-qb$. If it were nonzero, its smaller Euclidean value would contradict the choice of $b$. Thus $r=0$ and every $a\in I$ lies in $(b)$. Conversely $(b)\subseteq I$ because $I$ is an ideal. Hence $I=(b)$. The zero ideal is already $(0)$, proving **[every Euclidean domain is a principal ideal domain](../../../../every-euclidean-domain-is-a-principal-ideal-domain.md)**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
