<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [divide-and-conquer asymptotic expansion](../../../../../../divide-and-conquer-asymptotic-expansion.md) separates the $x=O(a)$ endpoint region from the $x=O(1)$ bulk, whose expansions individually contain terms that are nonuniform in the other region. Here the recombined answer can also be checked exactly. Put $y=\sqrt{a+x}$; then

$$
I(a)=2\int_{\sqrt a}^{\infty}\frac{dy}{y^2+1-a}
=\frac{\pi-2\arctan\sqrt{a/(1-a)}}{\sqrt{1-a}}.
$$

As $a\to0^+$,

$$
\arctan\sqrt{\frac a{1-a}}
=\sqrt a+O(a^{3/2}),
\qquad
(1-a)^{-1/2}=1+\frac a2+O(a^2).
$$

Multiplication gives

$$
\boxed{I(a)=\pi-2\sqrt a+\frac\pi2a+O(a^{3/2}).}
$$

The nonanalytic $\sqrt a$ term is the contribution that a naive fixed-$x$ expansion misses at the endpoint.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
