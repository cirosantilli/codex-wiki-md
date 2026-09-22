<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

The convolution is

$$
(f*g)(x)=\int_{-\infty}^{\infty}f(x-y)g(y)\,dy.
$$

We claim that the $n$-fold convolution is

$$
\boxed{
F_n(x)=
\begin{cases}
\dfrac{x^{n-1}}{(n-1)!}e^{-x},&x\geq0,\\
0,&x<0.
\end{cases}}
$$

This is true for $n=1$. If it holds for $n-1$ and $x\geq0$, then

$$
\begin{aligned}
F_n(x)
&=\int_0^x e^{-(x-y)}
\frac{y^{n-2}e^{-y}}{(n-2)!}\,dy\\
&=\frac{e^{-x}}{(n-2)!}\int_0^xy^{n-2}\,dy
=\frac{x^{n-1}e^{-x}}{(n-1)!},
\end{aligned}
$$

and the convolution vanishes for $x<0$. This is the [gamma density from repeated exponential convolution](../../../../../gamma-density-from-repeated-exponential-convolution.md).

The Fourier transform is

$$
\boxed{
\widehat F_n(k)=\frac1{(n-1)!}
\int_0^\infty x^{n-1}e^{-(1+ik)x}\,dx
=\frac1{(1+ik)^n}}.
$$

The [convolution theorem](../../../../../convolution-theorem.md) states

$$
\boxed{\widehat{f*g}(k)=\widehat f(k)\widehat g(k)}.
$$

Indeed, Fubini and $u=x-y$ give

$$
\begin{aligned}
\widehat{f*g}(k)
&=\int\!\int e^{-ikx}f(x-y)g(y)\,dy\,dx\\
&=\int\!\int e^{-ik(u+y)}f(u)g(y)\,du\,dy
=\widehat f(k)\widehat g(k).
\end{aligned}
$$

Since $\widehat F(k)=(1+ik)^{-1}$, induction immediately verifies

$$
\widehat F_n=(\widehat F)^n=(1+ik)^{-n}.
$$

For [Parseval identity](../../../../../parseval-identity.md), take $g(x)=\overline{f(-x)}$. Then

$$
(f*g)(0)=\int_{-\infty}^{\infty}|f(x)|^2\,dx,
\qquad
\widehat g(k)=\overline{\widehat f(k)}.
$$

Using Fourier inversion at zero, which follows from the supplied delta identity,

$$
(f*g)(0)=\frac1{2\pi}\int_{-\infty}^{\infty}
\widehat{f*g}(k)\,dk,
$$

and the convolution theorem gives

$$
\boxed{
\int_{-\infty}^{\infty}|f(x)|^2\,dx
=\frac1{2\pi}\int_{-\infty}^{\infty}|\widehat f(k)|^2\,dk}.
$$

Apply this to $F_{n+1}$. Since

$$
\int_0^\infty|F_{n+1}(x)|^2dx
=\frac1{(n!)^2}\int_0^\infty x^{2n}e^{-2x}\,dx
=\frac{(2n)!}{2^{2n+1}(n!)^2},
$$

one obtains the [Even rational Parseval integral](../../../../../even-rational-parseval-integral.md)

$$
\boxed{
\int_{-\infty}^{\infty}\frac{dk}{(1+k^2)^{n+1}}
=\frac{\pi(2n)!}{2^{2n}(n!)^2}
=\frac\pi{4^n}\binom{2n}{n}}.
$$

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
