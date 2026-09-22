<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [Fourier cosine series](../../../../../../../fourier-cosine-series.md), first take the [even extension](../../../../../../../even-extension.md) $F_e(x)=f(|x|)$ on $[-\pi,\pi]$, and then its $2\pi$-[periodic extension](../../../../../../../periodic-extension.md). Evenness eliminates the [sine](../../../../../../../sine.md) terms. With the constant term written as $a_0/2$, the [Fourier coefficients](../../../../../../../fourier-coefficient.md) and [series](../../../../../../../series-mathematics.md) are

$$
\boxed{a_n=\frac2\pi\int_0^\pi f(x)\cos(nx)\,dx\quad(n=0,1,2,\ldots),\qquad
\frac{a_0}{2}+\sum_{n=1}^\infty a_n\cos(nx).}
$$

For the [Fourier sine series](../../../../../../../fourier-sine-series.md), take the [odd extension](../../../../../../../odd-extension.md) $F_o(x)=f(x)$ for $0<x<\pi$ and $F_o(x)=-f(-x)$ for $-\pi<x<0$, and extend with period $2\pi$. Values assigned at isolated endpoints do not change the [Fourier coefficients](../../../../../../../fourier-coefficient.md). Oddness eliminates the constant and [cosine](../../../../../../../cosine.md) terms, leaving

$$
\boxed{b_n=\frac2\pi\int_0^\pi f(x)\sin(nx)\,dx\quad(n\geq1),\qquad
\sum_{n=1}^\infty b_n\sin(nx).}
$$

Both formulas follow by [orthogonality](../../../../../../../orthogonal-vectors.md) on $[-\pi,\pi]$ and the parity of the extensions.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
