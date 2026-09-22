<h1 id="41d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Pair the two entries of the even-reflected sequence that contain $x_n$. For every $k$,

$$
\begin{aligned}
Y_k
&=\sum_{n=0}^{N-1}x_n
\left(e^{-\pi ink/N}+e^{-\pi i(2N-1-n)k/N}\right)\\
&=\sum_{n=0}^{N-1}x_n
\left(e^{-\pi ink/N}+e^{\pi i(n+1)k/N}\right)\\
&=2e^{\pi ik/(2N)}
\sum_{n=0}^{N-1}x_n
\cos\left(\frac{\pi}{N}\left(n+\frac12\right)k\right).
\end{aligned}
$$

Consequently

$$
\boxed{\frac12e^{-\pi ik/(2N)}Y_k
=\sum_{n=0}^{N-1}x_n
\cos\left(\frac{\pi}{N}\left(n+\frac12\right)k\right)}
$$

for $0\leq k<2N$, as required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41D](../../41d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
