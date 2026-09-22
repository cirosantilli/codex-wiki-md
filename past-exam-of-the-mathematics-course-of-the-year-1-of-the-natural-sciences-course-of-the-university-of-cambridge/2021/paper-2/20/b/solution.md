<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With homogeneous [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), the eigenfunctions are $\sin(n\pi x/L)$ and all modes decay. Write

$$
\Theta(x,t)=\sum_{n=1}^{\infty}b_n\sin\frac{n\pi x}{L}
\,e^{-\kappa(n\pi/L)^2t},\qquad
b_n=\frac{2T_0}{L}\int_0^L\sin^2\frac{\pi x}{L}\sin\frac{n\pi x}{L}\,dx.
$$

Reflection about the midpoint makes every even-$n$ coefficient zero. For odd $n$, putting $u=\pi x/L$ and using the product-to-sum identity gives

$$
\begin{aligned}
b_n&=\frac{2T_0}{\pi}\int_0^\pi\sin^2u\sin(nu)\,du\\
&=\frac{2T_0}{\pi}\left[\frac1n-\frac12\left(\frac1{n+2}+\frac1{n-2}\right)\right]
=\frac{8T_0}{\pi n(4-n^2)}.
\end{aligned}
$$

In particular $b_1=8T_0/(3\pi)$ and $b_3=-8T_0/(15\pi)$. Thus

$$
\boxed{\Theta(x,t)=\frac{8T_0}{\pi}
\sum_{m=0}^{\infty}
\frac{\sin((2m+1)\pi x/L)}{(2m+1)[4-(2m+1)^2]}
\,e^{-\kappa(2m+1)^2\pi^2t/L^2}.}
$$

This uses the [Fourier sine series of a squared sine](../../../../../fourier-sine-series-of-a-squared-sine.md). The coefficients are $O(n^{-3})$, so the initial series converges uniformly; for $t>0$ the exponential factors also justify termwise differentiation to check the [heat equation](../../../../../heat-equation.md). Every mode vanishes at both endpoints, and the initial series gives the specified profile. Unlike part (a), there is no constant mode: the temperature tends to zero, with leading long-time term

$$
\Theta(x,t)\sim\frac{8T_0}{3\pi}\sin\frac{\pi x}{L}\,e^{-\kappa\pi^2t/L^2}.
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
