<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $N=\sqrt{(0)}$. Every element of the [extension of an ideal](../../../../extension-of-an-ideal.md) $NR_{\mathfrak p}$ is a fraction $a/s$ with $a\in N$ and $s\notin\mathfrak p$: a finite sum of such fractions has a common denominator and numerator still in the [ideal](../../../../ideal.md) $N$. If $a^n=0$, then $(a/s)^n=0$, so

$$
NR_{\mathfrak p}\subseteq\sqrt{(0)_{R_{\mathfrak p}}}.
$$

Conversely, let $a/s$ be a [nilpotent element](../../../../nilpotent.md) of the [localization at a prime ideal](../../../../localization-at-a-prime-ideal.md) $R_{\mathfrak p}$. For some $n\geq1$, $a^n/s^n=0$. The [vanishing criterion in a module localization](../../../../vanishing-criterion-in-a-module-localization.md) supplies $t\notin\mathfrak p$ with $ta^n=0$. It follows that

$$
(ta)^n=t^{n-1}(ta^n)=0,
$$

so $ta\in N$. Since $ts\notin\mathfrak p$,

$$
\frac as=\frac{ta}{ts}\in NR_{\mathfrak p}.
$$

This proves that the [nilradical commutes with localization](../../../../nilradical-commutes-with-localization.md):

$$
\boxed{\operatorname{Nil}(R_{\mathfrak p})=NR_{\mathfrak p}.}
$$

The multiplication by $t$ is necessary: the numerator $a$ of a [nilpotent element](../../../../nilpotent.md) in a [localization](../../../../localization-of-a-ring.md) need not itself be [nilpotent](../../../../nilpotent.md) in $R$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
