<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The truncated [Perron formula](../../../../../../perron-s-formula.md) says that, for $c>1$ and $T\geq2$,

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-iT}^{c+iT}
\left(\sum_{n=1}^\infty\frac{a_n}{n^s}\right)\frac{x^s}{s}\,ds
+\text{a truncation error},
$$

where an endpoint has half weight and the error is controlled by

$$
\sum_n|a_n|\left(\frac xn\right)^c
\min\left(1,\frac1{T|\log(x/n)|}\right).
$$

Apply this with $a_n=\mu(n)$, $c=1+1/\log x$, and

$$
T=\exp(\sqrt{\log x}).
$$

Part (b) makes the integrand $x^s/(s\zeta(s))$. Move the contour to

$$
\sigma_0=1-\frac{c_2}{\log T}
=1-\frac{c_2}{\sqrt{\log x}},
$$

using a contour that stays inside the [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md) near small $|t|$. The estimates supplied in the question give $1/\zeta(s)\ll\log(|t|+3)$ on the new contour. Its vertical segment is therefore

$$
\ll x^{\sigma_0}(\log T)^2
\ll x\exp(-c_3\sqrt{\log x}),
$$

after decreasing $c_3$. The horizontal segments and the Perron truncation error are

$$
\ll\frac{x(\log x)^{O(1)}}T
\ll x\exp(-c_4\sqrt{\log x}).
$$

No residue is crossed because $1/\zeta(s)$ has a zero, rather than a pole, at $s=1$. Thus the [Mertens function](../../../../../../mertens-function.md) satisfies

$$
\boxed{\sum_{n\leq x}\mu(n)
\ll x\exp(-c\sqrt{\log x})}
$$

for some absolute $c>0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
