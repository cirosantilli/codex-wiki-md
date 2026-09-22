<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Fourier cosine series](../../../../../../../fourier-cosine-series.md) on $[0,L]$ is

$$
f(x)\sim\frac{a_0}{2}+\sum_{n=1}^\infty a_n\cos\frac{n\pi x}{L},
\qquad
\boxed{a_n=\frac2L\int_0^Lf(x)\cos\frac{n\pi x}{L}\,dx\quad(n\geq0).}
$$

It is the [Fourier series](../../../../../../../fourier-series-split.md) of the [even extension](../../../../../../../even-extension.md) to $[-L,L]$, repeated with [period](../../../../../../../period-of-a-function.md) $2L$. The [Fourier sine series](../../../../../../../fourier-sine-series.md) is

$$
f(x)\sim\sum_{n=1}^\infty b_n\sin\frac{n\pi x}{L},
\qquad
\boxed{b_n=\frac2L\int_0^Lf(x)\sin\frac{n\pi x}{L}\,dx\quad(n\geq1).}
$$

It comes from the [odd extension](../../../../../../../odd-extension.md) and its $2L$-[periodic extension](../../../../../../../periodic-extension.md). These [Fourier coefficient](../../../../../../../fourier-coefficient.md) formulas follow by [Fourier orthogonality](../../../../../../../fourier-orthogonality.md), since every nonconstant [sine](../../../../../../../sine.md) or [cosine](../../../../../../../cosine.md) has squared [integral](../../../../../../../integral-split.md) $L/2$ on $[0,L]$, while the [constant function](../../../../../../../constant-function.md) has squared [integral](../../../../../../../integral-split.md) $L$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
