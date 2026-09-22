<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $q=e^{i\theta}/2$. The required sine sum is the [imaginary part](../../../../imaginary-part.md) of a finite [geometric series](../../../../geometric-series.md):

$$
\sum_{n=1}^Nq^n=\frac{q(1-q^N)}{1-q}
=\frac{(q-q^{N+1})(1-\overline q)}{|1-q|^2}.
$$

The denominator is $(5-4\cos\theta)/4$. The numerator's [imaginary part](../../../../imaginary-part.md) is

$$
\frac12\sin\theta-\frac{\sin((N+1)\theta)}{2^{N+1}}
+\frac{\sin(N\theta)}{2^{N+2}}.
$$

Dividing and multiplying numerator and denominator by $2^N$ proves

$$
\boxed{\sum_{n=1}^N\frac{\sin(n\theta)}{2^n}
=\frac{2^{N+1}\sin\theta+\sin(N\theta)-2\sin((N+1)\theta)}{2^N(5-4\cos\theta)}.}
$$

For real $\theta$, $5-4\cos\theta\ge1$, so there is no exceptional angle requiring a limiting interpretation. At $N=1$ the expression reduces to $\sin\theta/2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
