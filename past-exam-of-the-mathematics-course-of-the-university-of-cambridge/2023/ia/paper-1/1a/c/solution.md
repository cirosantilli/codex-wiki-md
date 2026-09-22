<h1 id="1a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since

$$
\mathcal F^{-1}[e^{ika}]=\delta(x+a),
\qquad
\mathcal F^{-1}[e^{-ika}]=\delta(x-a),
$$

the [Inverse Fourier transforms of phase factors](../../../../../../inverse-fourier-transforms-of-phase-factors.md) give

$$
\boxed{
\mathcal F^{-1}[\cos(ka)]
=\frac12\bigl[\delta(x+a)+\delta(x-a)\bigr]
}
$$

and

$$
\boxed{
\mathcal F^{-1}[\sin(ka)]
=\frac1{2i}\bigl[\delta(x+a)-\delta(x-a)\bigr].
}
$$

From $z=\tan w=-i(e^{2iw}-1)/(e^{2iw}+1)$ one obtains

$$
e^{2iw}=\frac{1+iz}{1-iz},
\qquad
w=\frac1{2i}\log\frac{1+iz}{1-iz}.
$$

For $z=(2\sqrt3-3i)/7$ the quotient is $1+i\sqrt3=2e^{i\pi/3}$. Its principal logarithm is $\log2+i\pi/3$, so the principal value is

$$
\boxed{\tan^{-1}z=\frac\pi6-\frac i2\log2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1A](../../1a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
