<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Bessel process](../../../../../../bessel-process.md)

$$
dX_t=dB_t+\frac{d-1}{2X_t}dt,
$$

the [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md) is $s(x)=x^{2-d}$ when $d\ne2$. If $0<\epsilon<x<R$, the [boundary hitting probability from a diffusion scale function](../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md) gives

$$
\mathbb P_x(T_R<T_\epsilon)
=\frac{s(x)-s(\epsilon)}{s(R)-s(\epsilon)}.
$$

If $d<2$, then $s(0)=0$ and $s(R)\to\infty$. Letting $\epsilon\downarrow0$ and then $R\to\infty$ shows that the process cannot escape to infinity before reaching zero. The exit time from each bounded interval is finite almost surely, so $T_0<\infty$ almost surely.

If $d>2$, then $s(\epsilon)\to\infty$ in absolute value as $\epsilon\downarrow0$. Equivalently,

$$
\mathbb P_x(T_\epsilon<T_R)
=\frac{s(R)-s(x)}{s(R)-s(\epsilon)}
\longrightarrow0.
$$

**Thus the process does not hit zero. The borderline case $d=2$ has scale function $\log x$ and also does not hit zero. This is the [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
