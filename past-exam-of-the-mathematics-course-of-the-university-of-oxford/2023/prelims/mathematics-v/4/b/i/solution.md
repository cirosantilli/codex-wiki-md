<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $a=\pi/2$. The constant [Fourier coefficient](../../../../../../../fourier-coefficient.md) is

$$
a_0=\frac2\pi\left(\int_0^a x\,dx+\int_a^\pi a\,dx\right)=\frac{3\pi}{4}.
$$

For $n\geq1$, [integration by parts](../../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\int_0^a x\cos(nx)\,dx
&=\frac{a\sin(na)}n+\frac{\cos(na)-1}{n^2},\\
\int_a^\pi a\cos(nx)\,dx&=-\frac{a\sin(na)}n.
\end{aligned}
$$

The $n^{-1}$ terms cancel. Thus

$$
a_n=\frac{2}{\pi n^2}\left(\cos\frac{n\pi}{2}-1\right),\qquad
\boxed{f(x)=\frac{3\pi}{8}+\frac2\pi\sum_{n=1}^\infty
\frac{\cos(n\pi/2)-1}{n^2}\cos(nx)\quad(0\leq x\leq\pi).}
$$

This [Fourier cosine series](../../../../../../../fourier-cosine-series.md) has $a_n=0$ when $n$ is divisible by four, $a_n=-4/(\pi n^2)$ when $n\equiv2\pmod4$, and $a_n=-2/(\pi n^2)$ when $n$ is odd.

Similarly,

$$
\begin{aligned}
\int_0^a x\sin(nx)\,dx&=-\frac{a\cos(na)}n+\frac{\sin(na)}{n^2},\\
\int_a^\pi a\sin(nx)\,dx&=\frac{a\cos(na)}n-\frac{a(-1)^n}n.
\end{aligned}
$$

Therefore

$$
b_n=\frac{2\sin(n\pi/2)}{\pi n^2}-\frac{(-1)^n}{n},\qquad
\boxed{f(x)=\sum_{n=1}^\infty\left(\frac{(-1)^{n+1}}n+
\frac{2\sin(n\pi/2)}{\pi n^2}\right)\sin(nx)\quad(0<x<\pi).}
$$

The [Fourier sine series](../../../../../../../fourier-sine-series.md) also equals $f(0)=0$ at zero, but has value zero at $\pi$, where $f(\pi)=\pi/2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
