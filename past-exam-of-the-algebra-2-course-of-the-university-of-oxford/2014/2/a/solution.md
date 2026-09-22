<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero integer-coefficient [polynomial](../../../../polynomial-split.md) $F$, its [polynomial content](../../../../polynomial-content.md) $c(F)$ is the positive [greatest common divisor](../../../../greatest-common-divisor.md) of all its coefficients; one may set $c(0)=0$. A [primitive polynomial](../../../../primitive-polynomial.md) has content one.

For $f\in\mathbb Q[t]\setminus\{0\}$, choose a positive integer $m$ clearing its denominators, so $F=mf\in\mathbb Z[t]$. Put $d=c(F)>0$. Then

$$
f=\frac dm\frac Fd,
$$

where $f_1=F/d$ is an integer-coefficient [primitive polynomial](../../../../primitive-polynomial.md). This proves existence with $\alpha=d/m>0$.

For uniqueness, suppose $\alpha f_1=\beta g_1$, where both integer-coefficient polynomials are primitive and $\alpha,\beta>0$. Write $\alpha/\beta=a/b$ in lowest terms with $a,b$ positive. Then $g_1=(a/b)f_1$ has integer coefficients. Coprimality forces $b$ to divide every coefficient of $f_1$, hence $b=1$. Now $g_1=af_1$ has content $a$, so $a=1$. Therefore $\alpha=\beta$ and $f_1=g_1$.

Define the [rational polynomial content](../../../../rational-polynomial-content.md) by this unique positive multiplier. If $f=\alpha f_1$ and $g=\beta g_1$, [Gauss lemma for polynomials](../../../../gauss-lemma-for-polynomials.md) says that $f_1g_1$ is primitive. Thus

$$
fg=(\alpha\beta)(f_1g_1),\qquad
\boxed{c(fg)=c(f)c(g).}
$$

The uniqueness argument also shows that the construction is independent of the chosen denominator-clearing integer $m$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
