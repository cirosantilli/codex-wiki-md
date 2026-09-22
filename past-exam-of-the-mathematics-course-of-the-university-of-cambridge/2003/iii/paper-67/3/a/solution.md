<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a genuine indexing defect in the printed PDF: its new value is at $m+1$, while every old-time coefficient is centered at $m$. On a fixed grid the literal residual contains

$$
\frac{u(x+\delta,t+k)-u(x,t)}k-L_\delta u(x,t)
=\frac\delta k u_x+O(1)+O(k)+O(\delta^2),\qquad k=\mu\delta^2.
$$

For a general solution the leading term is $u_x/(\mu\delta)$, so this is not a consistent diffusion discretization. It also leaves one new interior value unspecified while imposing a generally incompatible update on a prescribed boundary value. The calculation that follows is for the intended same-node update $U_m^{n+1}=U_m^n+kL_\delta U_m^n$; that correction is necessary, not an unnoticed transcription change.

For the [midpoint flux stencil for one-dimensional diffusion](../../../../../../midpoint-flux-stencil-for-one-dimensional-diffusion.md), define

$$
L_\delta u(x)=\frac{a(x-\delta/2)[u(x-\delta)-u(x)]+a(x+\delta/2)[u(x+\delta)-u(x)]}{\delta^2}.
$$

Assume sufficient smoothness of $a$ and the solution for the displayed remainders. Multiplying the centered [Taylor expansions](../../../../../../taylor-expansion.md) of $a$ and $u$ gives

$$
L_\delta u=(au_x)_x+\delta^2\left(\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a^{(3)}u_x}{24}\right)+O(\delta^4).
$$

The first time difference is $(u(t+k)-u(t))/k=u_t+ku_{tt}/2+O(k^2)$. After using the [diffusion equation](../../../../../../diffusion-equation-split.md), the [normalized local truncation error](../../../../../../normalized-local-truncation-error.md) is

$$
\tau_m^n=\frac{k}{2}u_{tt}-\delta^2\left(\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a^{(3)}u_x}{24}\right)+O(k^2+\delta^4).
$$

Therefore, for the corrected update,

$$
\boxed{\tau=O(k+\delta^2),\qquad d=k\tau=O(k^2+k\delta^2).}
$$

The first is the residual divided by the time step; the second is the unnormalized one-step defect. At fixed $\mu=k/\delta^2$ they are respectively $O(\delta^2)$ and $O(\delta^4)$. A rate based on derivatives is not justified for a merely bounded nonsmooth $a$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
