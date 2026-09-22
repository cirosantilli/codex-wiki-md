<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Transverse force balance on a short element gives

$$
\rho y_{tt}=\tau y_{xx},\qquad c=\sqrt{\tau/\rho}.
$$

With fixed ends,

$$
y(x,t)=\sum_{n\ge1}[A_n\cos(\omega_nt)+B_n\sin(\omega_nt)]\sin\frac{n\pi x}{L},
\quad\omega_n=\frac{n\pi c}{L}.
$$

Here $A_n=0$. If $b_n$ are the sine coefficients of initial [velocity](../../../../../velocity.md), then

$$
b_n=\frac{4v}{n\pi\sqrt\varepsilon}\sin\frac{n\pi l}{L}\sin\frac{n\pi\varepsilon}{2L},
\qquad B_n=\frac{b_n}{\omega_n}.
$$

The total deposited energy is $E=\rho v^2/2$, while

$$
\frac{E_n}{E}=\frac{8L}{n^2\pi^2\varepsilon}
\sin^2\frac{n\pi l}{L}\sin^2\frac{n\pi\varepsilon}{2L}.
$$

The seventh mode is eliminated by striking at a node $l=jL/7$, $j=1,\ldots,6$. For a narrow hammer, each fixed-mode fraction is $O(\varepsilon)$; beyond the inverse-width cutoff the envelope falls as $n^{-2}$, modulated by the two sine factors.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
