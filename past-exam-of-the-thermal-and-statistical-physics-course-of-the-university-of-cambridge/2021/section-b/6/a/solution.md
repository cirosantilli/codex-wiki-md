<h1 id="section-b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let each step have [length](../../../../../length.md) $a$, and let $K$ be the number of right steps among $N$ independent steps. Then $K$ has a [binomial distribution](../../../../../binomial-distribution.md) and the physical displacement is $x=a[K-(N-K)]=a(2K-N)$. Therefore $K=(N+x/a)/2$, and the position [probability mass](../../../../../probability-mass.md) is

$$
\boxed{P_{\rm 1D}(x,N)=\binom{N}{(N+x/a)/2}
 w_+^{(N+x/a)/2}w_-^{(N-x/a)/2}.}
$$

This is zero unless $x/a$ is an integer, $|x/a|\leq N$, and $N+x/a$ is even. The parity condition matters because the walk alternates between the two sublattices. If distance is measured in lattice spacings, replace $x/a$ by $x$.

Normalization follows from the [binomial theorem](../../../../../binomial-theorem.md). Its first two [moments](../../../../../moment.md) provide useful checks:

$$
\langle x\rangle=Na(w_+-w_-),\qquad
\operatorname{Var}(x)=4Na^2w_+w_-=Na^2\left[1-(w_+-w_-)^2\right].
$$

These are exact discrete-time statements; a smooth continuum [probability density](../../../../../probability-density.md) requires coarse-graining over the lattice and its parity oscillation.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
