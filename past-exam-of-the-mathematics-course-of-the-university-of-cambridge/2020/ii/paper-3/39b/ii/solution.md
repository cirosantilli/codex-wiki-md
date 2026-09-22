<h1 id="39b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $x=Vt$ with fixed $V>0$. The relevant [stationary point](../../../../../../stationary-point.md) will have $k=O(V^2/S^2)$, so the assumption $\epsilon V^2/S^2\ll1$ allows the long-wave approximation

$$
\sin(k\epsilon)\sim k\epsilon.
$$

Using $\sin A\cos B=[\sin(A+B)+\sin(A-B)]/2$, the phase $Sk^{3/2}+Vk$ has no stationary point for $k>0$. The other phase is

$$
\phi(k)=Sk^{3/2}-Vk,
$$

with

$$
\phi'(k_0)=0,
\qquad
k_0=\frac{4V^2}{9S^2},
$$

and

$$
\phi(k_0)=-\frac{4V^3}{27S^2},
\qquad
\phi''(k_0)=\frac{9S^2}{8V}>0.
$$

The stationary part of the integral is therefore

$$
-\frac{W\epsilon}{\pi S}
\int_0^\infty k^{-3/2}\sin[t\phi(k)]\,dk.
$$

By the [one-dimensional stationary-phase formula](../../../../../../one-dimensional-stationary-phase-formula.md), this is asymptotic to

$$
-\frac{W\epsilon}{\pi S}k_0^{-3/2}
\sqrt{\frac{2\pi}{t\phi''(k_0)}}
\sin\left(t\phi(k_0)+\frac\pi4\right).
$$

Since

$$
k_0^{-3/2}
\sqrt{\frac{2\pi}{t\phi''(k_0)}}
=\frac{9S^2\sqrt\pi}{2V^{5/2}\sqrt t},
$$

we obtain

$$
\eta(x,t)\sim
\frac{9W\epsilon S}{2\sqrt\pi V^{5/2}\sqrt t}
\sin\left(\frac{4V^3t}{27S^2}-\frac\pi4\right).
$$

Using $V=x/t$, this has the requested form

$$
\boxed{
\eta(x,t)\sim\frac{W\epsilon S t^2}{x^{5/2}}
F\!\left(\frac{x^3}{S^2t^2}\right)},
$$

where

$$
\boxed{F(q)=\frac9{2\sqrt\pi}
\sin\left(\frac{4q}{27}-\frac\pi4\right)}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [39B](../../39b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
