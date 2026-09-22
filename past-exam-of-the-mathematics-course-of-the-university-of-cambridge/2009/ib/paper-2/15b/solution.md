<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

For small transverse displacement, the [wave equation on a string](../../../../../wave-equation-on-a-string.md) is

$$
\boxed{y_{tt}=c^2y_{xx},\qquad c^2=T/\rho,}
$$

where $T$ is the tension and $\rho$ is mass per unit length. Using [separation of variables](../../../../../separation-of-variables.md), put $y=X(x)F(t)$, the ratios $X''/X=F''/(c^2F)$ equal a constant. The fixed-end conditions $X(0)=X(L)=0$ exclude nontrivial solutions for nonnegative separation constants; for $-\kappa^2$ they give $X=\sin(\kappa x)$ and $\kappa=n\pi/L$, $n\ge1$. The associated angular frequencies are $\omega_n=n\pi c/L$. Thus the general superposition of separated [normal modes](../../../../../normal-mode.md) is

$$
\boxed{y(x,t)=\sum_{n\ge1}\left[A_n\cos(\omega_nt)+B_n\sin(\omega_nt)\right]\sin\frac{n\pi x}{L}.}
$$

The string is initially straight and at rest before the impulse, so $A_n=0$. Assume the hammer interval lies inside $[0,L]$. The imposed velocity $g(x)=y_t(x,0)$ has [Fourier sine series](../../../../../fourier-sine-series.md) coefficient

$$
g_n=\frac{2v}{L}\int_{l-a/2}^{l+a/2}\sin\frac{n\pi x}{L}\,dx
=\frac{4v}{n\pi}\sin\frac{n\pi l}{L}\sin\frac{n\pi a}{2L}.
$$

Therefore $B_n=g_n/\omega_n$, giving the amplitude of every excited [normal mode](../../../../../normal-mode.md).

The string energy is $\frac\rho2\int_0^L(y_t^2+c^2y_x^2)\,dx$. At the impulse it is $E_{\mathrm{total}}=\rho av^2/2$. Orthogonality of the sine modes gives $E_n=\rho Lg_n^2/4$ initially; each mode subsequently exchanges kinetic and elastic energy while retaining that total. Thus the [modal energy of a localized velocity impulse on a string](../../../../../modal-energy-of-a-localized-velocity-impulse-on-a-string.md) has fractions

$$
\boxed{\frac{E_n}{E_{\mathrm{total}}}=\frac{8L}{a\pi^2n^2}\sin^2\frac{n\pi l}{L}\sin^2\frac{n\pi a}{2L}.}
$$

For $l=L/3$ and $a=L/10$, a mode is absent exactly when $\sin(n\pi/3)=0$ or $\sin(n\pi/20)=0$. Hence **the unexcited modes are precisely**

$$
\boxed{n\in3\mathbb N_{>0}\ \cup\ 20\mathbb N_{>0}.}
$$

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
