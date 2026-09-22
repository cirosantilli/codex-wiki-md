<h1 id="14d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The interval indicator has transform

$$
\boxed{\widetilde g(k)=\int_{-b}^be^{-ikx}\,dx=\frac{2\sin(bk)}k,}
$$

with [continuous](../../../../../../continuous-function.md) value $2b$ at $k=0$. By the [convolution theorem](../../../../../../convolution-theorem.md), $h=f*g$ has transform $4a\sin(bk)/[k(a^2+k^2)]$. Fourier inversion therefore expresses the requested integral as

$$
I(x):=\int_{\mathbb R}\frac{\sin(bk)e^{ikx}}{k(a^2+k^2)}\,dk
=\frac\pi{2a}h(x),\qquad h(x)=\int_{-b}^be^{-a|x-y|}\,dy.
$$

For $x>b$, $|x-y|=x-y$, so $h(x)=2e^{-ax}\sinh(ab)/a$. Symmetry gives the same expression with $|x|$ for $x<-b$. For $|x|\leq b$, splitting the integral at $y=x$ gives

$$
h(x)=\frac{1-e^{-a(x+b)}}a+\frac{1-e^{-a(b-x)}}a
=\frac2a\bigl(1-e^{-ab}\cosh(ax)\bigr).
$$

Consequently **the value for every real $x$ is**

$$
\boxed{I(x)=\begin{cases}
\displaystyle\frac\pi{a^2}\sinh(ab)e^{-a|x|},&|x|\geq b,\\[2mm]
\displaystyle\frac\pi{a^2}\left(1-e^{-ab}\cosh(ax)\right),&|x|\leq b.
\end{cases}}
$$

The two expressions agree at $x=\pm b$. This is the [exponential kernel convolved with an interval indicator](../../../../../../exponential-kernel-convolved-with-an-interval-indicator.md). The spectral integral is absolutely convergent: its apparent singularity at zero is removable, and the tail decays as $O(|k|^{-3})$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14D](../../14d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
