<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), put $\gamma=KW^2\sqrt{g/\rho_0}$. The [buoyancy-driven turbulent density diffusion](../../../../../../buoyancy-driven-turbulent-density-diffusion.md) equation gives, wherever $q=\bar\rho_z>0$,

$$
q_t=\gamma\partial_z^2(q^{3/2})=\frac{3\gamma}{4\sqrt q}\left[(q_z)^2+2q q_{zz}\right].
$$

The coefficient outside the bracket is positive, so the local [density gradient](../../../../../../density-gradient.md) increases precisely when

$$
\boxed{(\bar\rho_{zz})^2+2\bar\rho_z\bar\rho_{zzz}>0.}
$$

At a point where $q=0$, use the original degenerate diffusion equation rather than dividing by $\sqrt q$.

For the proposed [self-similar solution](../../../../../../similarity-solution.md), $\bar\rho=\rho_0[1+F(t)G(z)]$ and $F(0)=1$. Substitution into $\bar\rho_t=\partial_zF_\rho$ gives

$$
\rho_0F'G=\gamma\rho_0^{3/2}F^{3/2}\frac{d}{dz}\left[(G')^{3/2}\right].
$$

An odd power profile $G(z)=C\operatorname{sgn}(z)|z|^p$ has right-hand spatial power $(3p-5)/2$. Matching it to $p$ requires $p=5$. Thus choose $G=Cz^5$ with $C>0$, an odd, increasing profile. Since $G'=5Cz^4$, its flux is proportional to $z^6$ on both sides of the midplane. The resulting [quintic density-profile similarity in an unstable tube](../../../../../../quintic-density-profile-similarity-in-an-unstable-tube.md) satisfies

$$
F'=A F^{3/2},\qquad A=6\,5^{3/2}KW^2\sqrt{gC}.
$$

Integration gives $F^{-1/2}=1-At/2$. Consequently

$$
\boxed{\bar\rho(z,t)=\rho_0\left[1+\frac{Cz^5}{(1-t/t_*)^2}\right],\qquad t_*=\frac{1}{3\,5^{3/2}KW^2\sqrt{gC}},\quad 0\le t<t_*.}
$$

Although mixing transports density downwards, the local [density gradient](../../../../../../density-gradient.md) can grow because spatial variations of the flux redistribute density. In this example the downward flux increases towards each end, driving the formal amplification of the odd profile.

This [self-similar solution](../../../../../../similarity-solution.md) deliberately ignores the end conditions: its nonzero end flux cannot satisfy impermeable ends. Moreover, the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) requires $F C|z|^5\ll1$, which fails before the formal divergence. A closed tube has only finite available [potential energy](../../../../../../potential-energy.md), so it cannot sustain indefinitely growing [turbulent kinetic energy](../../../../../../turbulent-kinetic-energy.md) or the assumed instantaneous flux law. End effects, changing eddy statistics and decay of the unstable stratification must eventually replace this local model. The conflicting endpoint labels in the source do not enter the calculation because end conditions have been expressly excluded.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
