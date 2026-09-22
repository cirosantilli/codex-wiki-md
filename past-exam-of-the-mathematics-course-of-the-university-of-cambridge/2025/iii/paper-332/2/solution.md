<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $K=k\Delta\rho g/\mu$. [Hydrostatic pressure](../../../../../hydrostatic-pressure.md) continuity at the lower boundary of the light current gives

$$
p(x,z,t)=p_H-\rho g(H-z)+\Delta\rho g\,[h(x,t)-z]
$$

inside the current, so $p_x=\Delta\rho g h_x$. [Darcy law](../../../../../darcy-law.md) gives the depth-integrated horizontal flux per unit transverse width

$$
q=-Kh h_x.
$$

Thus the [porous gravity current](../../../../../porous-gravity-current.md) satisfies

$$
\boxed{\phi h_t+q_x=0,
\qquad q=-\frac{k\Delta\rho g}{\mu}hh_x}
$$

away from the fracture. The boundary and front conditions are

$$
q(0,t)=Q,
\quad h(x_N,t)=0,
\quad q(x_N,t)=0.
$$

At $x=L$, the pressure excess at the base of the fracture is $\Delta\rho g h_L$. Taking upward leakage as positive,

$$
Q_l=\frac{W\alpha k\Delta\rho g}{\mu b}h_L,
\qquad
\boxed{q(L^+,t)=q(L^-,t)-Q_l.}
$$

This jump is the local [mass conservation](../../../../../mass-conservation.md) law for a [leaky porous gravity current](../../../../../leaky-porous-gravity-current.md).

At late times, $q=Q$ to leading order on $0<x<L$, while $Q_l\simeq Q$. Integrating $q=-K(h^2)_x/2$ gives

$$
\boxed{
h(x)=\left[h_0^2-(h_0^2-h_L^2)\frac{x}{L}\right]^{1/2}.}
$$

Leakage balance and the pressure-driven drop determine

$$
\boxed{h_L=\frac{\mu bQ}{W\alpha k\Delta\rho g},}
\qquad
\boxed{h_0=\left(h_L^2+\frac{2\mu QL}{k\Delta\rho g}\right)^{1/2}.}
$$

In the far field, $h(L,t)\simeq h_L$ and

$$
\phi h_t=K(hh_x)_x.
$$

Balancing the two sides with $h=O(h_L)$ gives

$$
\boxed{x_N-L=O\left[\left(\frac{k\Delta\rho g h_L}{\phi\mu}t\right)^{1/2}\right].}
$$

More precisely, set

$$
h=h_L f(\eta),
\qquad
\eta=\frac{x-L}{(Kh_Lt/\phi)^{1/2}}.
$$

The [self-similar solution](../../../../../similarity-solution.md) is determined by

$$
(ff')'+\frac\eta2f'=0,
\qquad
f(0)=1,
\quad f(\eta_N)=0,
\quad ff'(\eta_N)=0,
$$

and $x_N=L+\eta_N(Kh_Lt/\phi)^{1/2}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
