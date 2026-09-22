<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $P=p/\rho_0$ and use the downward buoyancy anomaly $b=g\rho'/\rho_0$. This sign convention is required by the printed [potential vorticity](../../../../../potential-vorticity.md). The linear rotating [Boussinesq approximation](../../../../../boussinesq-approximation.md) gives

$$
u_t-fv=-P_x,\quad v_t+fu=-P_y,\quad w_t=-P_z-b,\quad b_t=N^2w,\quad u_x+v_y+w_z=0.
$$

Let $D=u_x+v_y$ and $\zeta=v_x-u_y$. Horizontal divergence and curl give $D_t-f\zeta=-\nabla_H^2P$ and $\zeta_t=-fD=fw_z$. Hence

$$
\nabla^2P=f\zeta-b_z,\qquad
q_t=\zeta_t-\frac f{N^2}b_{zt}=0.
$$

Thus the linear [potential vorticity](../../../../../potential-vorticity.md) is a time-independent field fixed by the initial data. Differentiate the pressure identity twice. Using $\zeta_{tt}=-f(P_{zz}+b_z)$ and $b_{ztt}=-N^2(P_{zz}+b_z)$ gives $\nabla^2P_{tt}=(N^2-f^2)(P_{zz}+b_z)$. Combining terms,

$$
\boxed{\nabla^2p_{tt}+f^2p_{zz}+N^2\nabla_H^2p
=\rho_0fN^2\left(\zeta-\frac f{N^2}b_z\right)=Q(\mathbf x).}
$$

The [linear pressure equation for rotating stratified flow](../../../../../linear-pressure-equation-for-rotating-stratified-flow.md) has source **$Q=\rho_0fN^2q$**. “Arbitrary” means that different initial potential-vorticity fields give different time-independent sources; it is not independent forcing that may vary in time. If buoyancy were instead defined upward as $-g\rho'/\rho_0$, both appearances of its sign would change consistently. The pressure source represents the balanced component alongside propagating [inertia-gravity waves](../../../../../inertia-gravity-wave.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
