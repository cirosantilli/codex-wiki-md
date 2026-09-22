<h1 id="10/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) bounds the lowest [eigenvalue](../../../../../eigenvalue.md) by the [Rayleigh quotient](../../../../../rayleigh-quotient.md) of any nonzero admissible trial function. For $f=1-(r/a)^p$, take $p>0$, which ensures boundedness, the outer [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), and finite radial Dirichlet energy. Direct [integration](../../../../../integral-split.md) gives

$$
\int_0^ar(f')^2dr=\frac p2,\qquad\int_0^arf^2dr=a^2\left[\frac12-\frac2{p+2}+\frac1{2p+2}\right]=\frac{a^2p^2}{2(p+1)(p+2)}.
$$

Therefore

$$
\lambda_1\leq\frac{(p+1)(p+2)}{a^2p}=\frac1{a^2}\left(p+3+\frac2p\right).
$$

The derivative is $1-2/p^2$, so the unique minimizing positive exponent is $p=\sqrt2$. This yields the [power-law variational bound for a circular membrane](../../../../../power-law-variational-bound-for-a-circular-membrane.md)

$$
\boxed{\lambda_1\leq\frac{3+2\sqrt2}{a^2},\qquad \nu_1\leq\frac{c(1+\sqrt2)}{2\pi a}\simeq0.384234\,\frac ca.}
$$

The optimizing function has zero derivative at the origin and is admissible for the energy principle despite its unbounded second derivative there. For comparison, the exact radial fundamental has $\sqrt{\lambda_1}a\simeq2.404826$, giving $\nu_1\simeq0.382740\,c/a$. The bound is about $0.39\%$ above this value.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
