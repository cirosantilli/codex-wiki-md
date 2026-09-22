<h1 id="9f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**No.** A standard counterexample comes from the [log-normal distribution](../../../../../../log-normal-distribution.md). Let

$$
f(x)=\frac1{x\sqrt{2\pi}}
\exp\left(-\frac{(\log x)^2}{2}\right),
\qquad x>0,
$$

and, for a fixed $0<|\varepsilon|\leq1$, let

$$
f_\varepsilon(x)
=f(x)\left[1+\varepsilon\sin(2\pi\log x)\right].
$$

This is a nonnegative density distinct from $f$. For every nonnegative integer $n$, substituting $z=\log x$ makes the difference of the $n$th moments proportional to

$$
\mathbb E[e^{nZ}\sin(2\pi Z)],
\qquad Z\sim N(0,1).
$$

It is the imaginary part of

$$
\mathbb E[e^{(n+2\pi i)Z}]
=\exp\left(\frac{(n+2\pi i)^2}{2}\right),
$$

which vanishes because its phase is $2\pi n$. The case $n=0$ also proves that $f_\varepsilon$ is normalized. Thus the two distributions have every finite moment equal but are different. Unbounded random variables need not be determined by their moments.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
