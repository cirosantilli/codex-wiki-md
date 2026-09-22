<h1 id="32c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [asymptotic sequence](../../../../../../asymptotic-sequence.md) satisfies

$$
\phi_{n+1}(x)=o(\phi_n(x))
\qquad(x\to x_0).
$$

The expansion  
$f\sim\sum_{n\geq0}a_n\phi_n$ means that for every $N\geq0$,

$$
f(x)-\sum_{n=0}^Na_n\phi_n(x)=o(\phi_N(x)).
$$

For $N=0$, division by $\phi_0$ gives

$$
a_0=\lim_{x\to x_0}\frac f{\phi_0}.
$$

For $n\geq1$, the definition with $N=n$ says

$$
f-\sum_{k=0}^{n-1}a_k\phi_k
=a_n\phi_n+o(\phi_n).
$$

Division by $\phi_n$ gives the second coefficient formula. In particular, asymptotic-expansion coefficients are unique.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32C](../../32c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
