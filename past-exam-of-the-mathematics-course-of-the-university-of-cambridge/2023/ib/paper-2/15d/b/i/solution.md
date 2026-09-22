<h1 id="15d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the spatial factors of the stationary [wavefunction](../../../../../../../wave-function.md) as

$$
\psi(x,t)=e^{-iEt/\hbar}
\begin{cases}
e^{ikx}+R e^{-ikx},&x<-a,\\
C e^{kx}+D e^{-kx},&-a<x<a,\\
T e^{ikx},&x>a,
\end{cases}
$$

where

$$
k=\frac{\sqrt{2mE}}{\hbar}.
$$

Since $U_0-E=E$, the decay constant inside the [potential barrier](../../../../../../../potential-barrier.md) is also $k$. Continuity of the [wavefunction](../../../../../../../wave-function.md) and its first [derivative](../../../../../../../derivative.md) at $x=-a$ and $x=a$ gives four linear equations. Solving them yields

$$
T=\frac{e^{-2ika}}{\cosh(2ka)}.
$$

Consequently the transmitted wave is

$$
\boxed{
\psi_{\rm tr}(x,t)
=\frac{\exp\!\left(i[k(x-2a)-Et/\hbar]\right)}
{\cosh(2ka)}
},
\qquad x>a,
$$

and its [probability density](../../../../../../../probability-density.md) is

$$
\boxed{
\rho_{\rm tr}(x,t)=|\psi_{\rm tr}|^2
=\operatorname{sech}^2(2ka)
}.
$$

This is [finite square barrier transmission at half barrier height](../../../../../../../finite-square-barrier-transmission-at-half-barrier-height.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [15D](../../../15d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
