<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After recharge stops, the finite interval sets the horizontal scale. Apply the [separable draining profile for power-law diffusion](../../../../../../separable-draining-profile-for-power-law-diffusion.md) to each limiting equation

$$
\phi h_t=D_m(h^m h_x)_x,\qquad (m,D_m)=(2,D)\ \hbox{or}\ (1,u_b),\qquad D=u_b\beta/2.
$$

With $\xi=x/L$ and virtual age $\tau=t+t_0$, the [similarity solution](../../../../../../similarity-solution.md) is

$$
h=\left(\frac{\phi L^2}{mD_m\tau}\right)^{1/m}F_m(\xi),\qquad (F_m^mF_m')'+F_m=0,\qquad F_m(0)=0,\qquad F_m'(1)=0.
$$

The positive profile fixes $c_m=\lim_{\xi\downarrow0}F_m^mF_m'=\int_0^1F_m\,d\xi$. The discharge follows either from the boundary [Darcy flux](../../../../../../darcy-velocity.md) or integrated [mass conservation](../../../../../../mass-conservation.md):

$$
Q_m=\frac{D_m}{L}\left(\frac{\phi L^2}{mD_m\tau}\right)^{(m+1)/m}c_m.
$$

In the deep regime this gives

$$
\boxed{h\propto\tau^{-1/2},\qquad Q_2=\frac{c_2\phi^{3/2}L^2}{2\sqrt{u_b\beta}}\tau^{-3/2}.}
$$

In the final shallow regime,

$$
\boxed{h\propto\tau^{-1},\qquad Q_1=\frac{c_1\phi^2L^3}{u_b}\tau^{-2}.}
$$

The deep profile contains the thin [outlet layer in a deep unconfined aquifer](../../../../../../outlet-layer-in-a-deep-unconfined-aquifer.md) described above. The whole aquifer eventually becomes shallow, and its nonzero basal permeability controls the ultimate $\tau^{-2}$ discharge.

Estimating the mobility crossover by a typical height $2/\beta$ gives

$$
\boxed{\tau_{\rm cross}\sim\frac{\phi\beta L^2}{u_b}.}
$$

Using the deep profile's height at the divide makes this $\tau_{\rm cross}\simeq\phi\beta L^2F_2(1)^2/(4u_b)$. These are regime-dependent similarity approximations: the virtual origins are set by matching to the initial drainage and crossover, and a deep regime occurs only if the aquifer is initially sufficiently deep.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
