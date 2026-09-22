<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
\phi(x)=\int_0^xu(t)\,dt,
\qquad
Au(x)=\frac{\phi(x)}x.
$$

The [Holder inequality](../../../../../../holder-inequality.md) gives

$$
|\phi(x)|^p x^{1-p}
\leq\int_0^x|u(t)|^p\,dt\longrightarrow0
\quad(x\downarrow0).
$$

Using $x^{-p}\,dx=-(p-1)^{-1}d(x^{1-p})$ and [integration by parts](../../../../../../integration-by-parts.md), while discarding the nonpositive boundary term at $x=1$, yields

$$
\begin{aligned}
\|Au\|_p^p
&=\int_0^1|\phi|^px^{-p}\,dx\\
&\leq\frac p{p-1}\int_0^1|\phi|^{p-1}x^{1-p}|u|\,dx\\
&=\frac p{p-1}\int_0^1|Au|^{p-1}|u|\,dx.
\end{aligned}
$$

Another application of [Hölder's inequality](../../../../../../holder-inequality.md) gives

$$
\|Au\|_p^p
\leq\frac p{p-1}\|Au\|_p^{p-1}\|u\|_p.
$$

After cancellation, with the zero case immediate,

$$
\boxed{\|Au\|_{L^p(0,1)}\leq\frac p{p-1}\|u\|_{L^p(0,1)}}.
$$

This is the [Hardy averaging inequality](../../../../../../hardy-averaging-inequality.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
