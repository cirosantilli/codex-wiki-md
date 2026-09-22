<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

In the fluid region $y>\eta(x)$, incompressibility and [potential flow](../../../../../potential-flow.md) give

$$
\nabla^2\phi=0,\qquad \nabla\phi\to0\quad(y\to\infty).
$$

No penetration through the exact surface gives

$$
(-\eta_x,1)\mathbin\cdot(U+\phi_x,\phi_y)=0,\qquad
\phi_y=(U+\phi_x)\eta_x\quad(y=\eta).
$$

The condition $hk\ll1$ says the hill slope is small; $|\nabla\phi|\ll U$ says the disturbance [velocity](../../../../../velocity.md) is small compared with the background wind. Dropping the product $\phi_x\eta_x$ and Taylor-shifting the boundary from $y=\eta$ to $y=0$ therefore gives

$$
\phi_y(x,0)=U\eta_x=-Uhk\sin kx.
$$

The decaying solution is

$$
\phi=Uh e^{-ky}\sin kx.
$$

Bernoulli's equation is

$$
p+\rho gy+\frac12\rho|Ue_x+\nabla\phi|^2=\text{constant}.
$$

To first order on the surface,

$$
p=\text{constant}-\rho g\eta-\rho U\phi_x,\qquad
\phi_x(x,0)=Uhk\cos kx.
$$

Thus

$$
p_{\rm trough}-p_{\rm crest}=2\rho h(g+kU^2).
$$

Equivalently, crest minus trough is the negative of this. For $kU^2/g\ll1$, hydrostatic elevation dominates; for $kU^2/g\gg1$, the Bernoulli [pressure](../../../../../pressure.md) drop caused by faster crest flow dominates.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
