<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h=\Delta x$, $k=\Delta t$ and $\mu=k/h$. For the exact solution $u(x,t)=F(x+t)$ of the [advection equation](../../../../../../transport-equation.md), the three left-hand samples are translations by $(\mu-1)h$, $\mu h$ and $(\mu+1)h$ relative to $(x_m,t_n)$; the right-hand samples are translations by zero and $h$.

Denote their coefficients by $a=\mu(1+\mu)/6$, $b=(2-\mu)(1+\mu)/3$, $c=(2-\mu)(1-\mu)/6$, $d=(2-\mu)/3$ and $e=(1+\mu)/3$. [Taylor expansion](../../../../../../taylor-expansion.md) compares moments

$$
M_j=a(\mu-1)^j+b\mu^j+c(\mu+1)^j-d\,0^j-e,
$$

where $0^0=1$ in the zeroth moment. Direct calculation gives

$$
M_0=M_1=M_2=M_3=0,\qquad
M_4=\frac{\mu(\mu-2)(\mu-1)(\mu+1)}3.
$$

Thus the unscaled exact-solution residual is

$$
\mathcal R_h=\frac{h^4}{72}\mu(\mu-2)(\mu-1)(\mu+1)u_{xxxx}+O(h^5).
$$

For fixed nonzero $\mu$, dividing by the time step yields

$$
\boxed{\frac{\mathcal R_h}{k}
=\frac{h^3}{72}(\mu-2)(\mu-1)(\mu+1)u_{xxxx}+O(h^4).}
$$

The scheme is therefore **third order under fixed-Courant refinement**, with an unscaled one-step defect of order four. Stability then gives third-order accumulated error for smooth data with [periodic boundary conditions](../../../../../../periodic-boundary-conditions.md). Calling the unscaled defect fourth order is a different convention, not fourth-order approximation of the differential equation.

At $\mu=-1,1,2$, the amplification factor in (b) becomes exactly $e^{i\mu\theta}$: the numerical step translates the grid data by that integer number of cells and is exact for this constant-speed [advection equation](../../../../../../transport-equation.md). At $\mu=0$ it is the identity, a zero-time-step limit. These are exact special shifts, rather than merely a cancellation of one term of the [Taylor expansion](../../../../../../taylor-expansion.md). This is the [implicit advection scheme with exact integer shifts](../../../../../../implicit-advection-scheme-with-exact-integer-shifts.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
