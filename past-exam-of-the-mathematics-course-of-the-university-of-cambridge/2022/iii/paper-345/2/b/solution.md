<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the concentration-dependent [reduced gravity](../../../../../../reduced-gravity-split.md)

$$
g'(\phi)=\frac g{\rho_0}(R_1\phi+R_2\phi^2),
\qquad
g'_\phi=\frac g{\rho_0}(R_1+2R_2\phi).
$$

Under the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), the three [shallow water equations](../../../../../../shallow-water-equations.md) can be written in advective form as

$$
\phi_t+u\phi_x=-\frac{\phi w_e}{h},
$$



$$
h_t+uh_x+hu_x=w_e-w_d,
$$



$$
u_t+uu_x+g'h_x+\frac h2g'_\phi\phi_x=-\frac{uw_e}{h}.
$$

The coefficient matrix of this [quasilinear system](../../../../../../quasilinear-system.md) has [characteristic speeds](../../../../../../characteristic-speed.md)

$$
\boxed{\lambda_0=u,\qquad \lambda_\pm=u\pm\sqrt{g'h}.}
$$

Thus this is a [hyperbolic system](../../../../../../hyperbolic-system.md) when $g'h>0$. Along the intermediate [characteristic curve](../../../../../../characteristic-curve.md) $dx/dt=u$, the concentration obeys

$$
\boxed{\frac{D\phi}{Dt}=\phi_t+u\phi_x=-\frac{\phi w_e}{h}.}
$$

It decreases because ambient entrainment dilutes the chemical; detrainment does not change the concentration of a well-mixed parcel.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
