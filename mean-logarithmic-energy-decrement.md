# Mean logarithmic energy decrement

↑ **Parent:** [Neutron moderation](neutron-moderation.md)

Consider a [nonrelativistic particle](nonrelativistic-particle.md) of [mass](mass.md) $m$ undergoing an [elastic collision](elastic-collision.md) with a stationary free target of [mass](mass.md) $M=Am$, where $A\geq1$. Assume the outgoing direction is uniformly distributed over solid angle in the [center of mass](center-of-mass.md) frame; this assumption concerns the [scattering angle](scattering-angle.md) distribution and need not hold for every target or [energy](energy-split.md). Let $\mu$ be the cosine of that frame's [scattering angle](scattering-angle.md). Transforming the outgoing [velocity](velocity.md) back to the laboratory gives

$$
x=\frac{E'}{E}=\frac{A^2+1+2A\mu}{(A+1)^2},\qquad
\alpha=\left(\frac{A-1}{A+1}\right)^2\leq x\leq1.
$$

The uniform distribution of $\mu$ on $[-1,1]$ makes $x$ uniform on $[\alpha,1]$. For $A>1$, integration yields

$$
\xi=\frac{1}{1-\alpha}\int_\alpha^1-\log x\,dx
=1+\frac{\alpha\log\alpha}{1-\alpha}.
$$

For equal [masses](mass.md), take the limit $\alpha\to0$: $\xi=1$. The [expected value](expected-value-split.md) of the fractional [energy](energy-split.md) after a collision is instead $\mathbb E[x]=(1+\alpha)/2$. These are different averages: averaging a [logarithm](logarithm.md) does not give the [logarithm](logarithm.md) of an average.

For independent collisions with the same distribution, the [logarithms](logarithm.md) of successive [energy](energy-split.md) ratios add. Thus

$$
\mathbb E[\log(E_n/E_0)]=-n\xi,\qquad
E_{\mathrm{geom}}=E_0e^{-n\xi},\qquad
n_{\mathrm{log}}=\frac{\log(E_0/E_*)}{\xi}.
$$

Here $E_{\mathrm{geom}}$ is the geometric-mean [energy](energy-split.md), and $n_{\mathrm{log}}$ is a characteristic collision count for reaching an [energy](energy-split.md) scale $E_*$. It is not an exact first-passage [expected value](expected-value-split.md). Individual histories fluctuate, and neither the time between collisions nor absorption is specified by this model.

In an original chosen example, set $E_0=10^6\,\mathrm{eV}$ and $E_*=0.025\,\mathrm{eV}$. Approximate [hydrogen](hydrogen.md) by $A=1$ and [carbon](carbon.md) by $A=12$. Then

$$
\begin{array}{c|c|c}
A&\xi&n_{\mathrm{log}}\\
1&1&17.50\\
12&0.15777&110.95
\end{array}
$$

These are illustrative model values, not measured collision counts from 1934. The [energy](energy-split.md) scale marks where neglected thermal motion matters; the calculation does not assert continued cooling to zero [energy](energy-split.md).

## ↑ Ancestors (9)

1. [Neutron moderation](neutron-moderation.md)
2. [Slow neutron](slow-neutron.md)
3. [Neutron](neutron-split.md)
4. [Nucleon](nucleon.md)
5. [Baryon](baryon.md)
6. [Hadron](hadron.md)
7. [Subatomic particle](subatomic-particle.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Neutron moderation](neutron-moderation.md)
