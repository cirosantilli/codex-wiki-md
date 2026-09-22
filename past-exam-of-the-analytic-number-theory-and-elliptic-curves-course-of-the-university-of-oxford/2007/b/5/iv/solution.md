<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose a nonzero [integer](../../../../../integer-split.md) $D$ with $D\alpha,D\beta\in\mathbb Z$. By the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), choose $z_n\in\mathbb Z$ satisfying $z_n\equiv D\alpha\pmod{q^n}$ and $z_n\equiv D\beta\pmod{r^n}$. Put $x_n=z_n/D$. Then

$$
|x_n-\alpha|_q\le|D|_q^{-1}q^{-n}\to0,\qquad
|x_n-\beta|_r\le|D|_r^{-1}r^{-n}\to0.
$$

This proves the requested simultaneous approximation, even when the rational targets have denominators divisible by either prime.

A [rational sequence converging to zero at every standard absolute value](../../../../../rational-sequence-converging-to-zero-at-every-standard-absolute-value.md) is:

$$
\boxed{y_n=\frac{n!}{1+(n!)^2}.}
$$

Its ordinary absolute value is at most $1/n!$, hence tends to zero. For a fixed prime $p$ and all sufficiently large $n$, the denominator is congruent to one modulo $p$, so $v_p(y_n)=v_p(n!)\to\infty$. Therefore $|y_n|_p\to0$ for each prime as well. The assertion concerns each fixed prime separately, rather than [uniform convergence](../../../../../uniform-convergence.md) over all primes.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
