<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

The [principle of stationary action](../../../../../principle-of-stationary-action.md), also called Hamilton's principle, requires $\delta\int_{t_1}^{t_2}L\,dt=0$ for fixed-endpoint path variations. Here the original PDF has $\dot r^2$ in the radial kinetic energy; the TeX has lost that dot. With $m>0$ and $r>0$, the [Lagrangian](../../../../../lagrangian.md) is

$$
L=\frac m2\dot r^2+\frac m2r^2\dot\phi^2-kmr^2.
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) for each coordinate gives

$$
\boxed{\ddot r=r\dot\phi^2-2kr,\qquad\frac d{dt}(mr^2\dot\phi)=0.}
$$

The two conserved quantities are [angular momentum](../../../../../angular-momentum.md) $h=mr^2\dot\phi$ and energy $E=\frac m2\dot r^2+\frac m2r^2\dot\phi^2+kmr^2$. By [Noether's theorem](../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md), they arise respectively from rotational invariance and time-translation invariance of the action. The coordinate $\phi$ is a [cyclic coordinate](../../../../../cyclic-coordinate.md), and $L$ has no explicit time dependence.

The [conjugate momentum](../../../../../canonical-momentum.md) for each coordinate is $p_r=m\dot r$, $p_\phi=mr^2\dot\phi$. The [Legendre transform](../../../../../convex-conjugate.md) $H=p_r\dot r+p_\phi\dot\phi-L$ gives the [Hamiltonian](../../../../../hamiltonian.md)

$$
\boxed{H=\frac{p_r^2}{2m}+\frac{p_\phi^2}{2mr^2}+kmr^2.}
$$

[Hamilton's equations](../../../../../hamilton-s-equations.md) are

$$
\dot r=\frac{p_r}{m},\quad \dot\phi=\frac{p_\phi}{mr^2},\quad
\dot p_r=\frac{p_\phi^2}{mr^3}-2kmr,\quad \dot p_\phi=0.
$$

Setting $p_\phi=h$ yields $m\ddot r=-V_{\rm eff}'(r)$ with the [effective potential](../../../../../effective-potential.md) $V_{\rm eff}=h^2/(2mr^2)+kmr^2$.

For $k>0$ and $h\ne0$, this potential tends to infinity both as $r\downarrow0$ and as $r\to\infty$, and has its unique stationary point at

$$
\boxed{r_0=\left(\frac{h^2}{2km^2}\right)^{1/4},\qquad V_{\rm eff}''(r_0)=8km>0.}
$$

The [effective potential stability criterion](../../../../../effective-potential-stability-criterion.md) proves a stable [circular orbit in a quadratic central potential](../../../../../circular-orbit-in-a-quadratic-central-potential.md), with $|\dot\phi|=\sqrt{2k}$. For a small radial displacement $\eta$, $\ddot\eta+8k\eta=0$ to first order, so radial perturbations oscillate rather than grow. The diagram shows the centrifugal and quadratic contributions and their sum in dimensionless units:

<a id="15d/image-the-effective-potential-for-a-central-force-orbit"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2-effective-potential.png)

**[Figure 1](#15d/image-the-effective-potential-for-a-central-force-orbit). The effective potential for a central-force orbit**.

The printed paper only says that $k$ is constant. Its claimed positive-radius stable circular orbit needs the additional attractive-force assumption $k>0$ and nonzero angular momentum. For $k<0$ there is no such minimum; for $k=0,h\ne0$ the effective potential is strictly decreasing. With $h=0,k>0$, the minimum is at the origin and is not a positive-radius circular orbit. These cases are not represented by the diagram.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
