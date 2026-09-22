<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

By the gravitational shell theorem, the inward acceleration at radius $r$ is $Gm(r)/r^2$, where $m(r)=4\pi\int_0^r\rho(s)s^2ds$. Force balance for a thin fluid shell gives $-\nabla P=\rho\nabla\Phi$, and hence

$$
\boxed{P'(r)=-Gm(r)\rho(r)/r^2.}
$$

Assembling shells from infinity gives $E_{\rm grav}=-\int_0^R Gm(r)\,dm(r)/r=-4\pi G\int_0^Rm\rho r\,dr$. Using the pressure equation and integration by parts yields

$$
E_{\rm grav}=4\pi\int_0^Rr^3P'(r)dr
=4\pi R^3P(R)-12\pi\int_0^Rr^2P(r)dr.
$$

For a star with negligible external pressure, $P(R)=0$, this is **$E_{\rm grav}=-3\langle P\rangle V$**. Nonzero external pressure would add the displayed surface term.

For a nonrelativistic [ideal gas](../../../../../ideal-gas.md), the virial relation is $E_{\rm grav}=-2E_{\rm kin}$ and total energy is negative. Under adiabatic compression its kinetic energy scales as $R^{-2}$, faster than the magnitude $R^{-1}$ of gravity, providing restoring support; its [adiabatic index](../../../../../heat-capacity-ratio.md) $5/3$ exceeds $4/3$. For an ultrarelativistic gas, $E_{\rm grav}=-E_{\rm kin}$ and both terms scale as $R^{-1}$, giving marginal stability at [adiabatic index](../../../../../heat-capacity-ratio.md) $4/3$ in this idealized Newtonian model. Corrections such as general relativity can then destabilize it.

Integrating the kinetic energy $p^2/(2m_p)$ over filled momentum states gives

$$
E_{\rm kin}=\frac{4\pi g_sV}{h^3}\int_0^{p_F}\frac{p^4}{2m_p}dp
=\frac{4\pi g_sVh^2}{10m_p}(p_F/h)^5.
$$

Since $p_F=h[3n/(4\pi g_s)]^{1/3}$, the pressure is

$$
P=\frac{h^2}{5m_p}\left(\frac3{4\pi g_s}\right)^{2/3}n^{5/3}
\sim\frac{h^2}{m_p}n^{5/3}.
$$

Finally $|E_{\rm grav}|\sim GM^2/R$, whereas $PV\sim(h^2/m_p)[M/(m_pR^3)]^{5/3}R^3$. Equating these by the [virial theorem](../../../../../virial-theorem.md) gives

$$
\boxed{R\sim\frac{h^2}{Gm_p^{8/3}}M^{-1/3}.}
$$

This is an order-of-magnitude estimate for nonrelativistic degeneracy support, not a uniform-density exact stellar solution.

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
