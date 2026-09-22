<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The neutral [displacement](../../../../../../displacement.md) equation gives, for each nonzero-frequency root,

$$
-i\omega\mathbf u_n=-\mu(\mathbf u_n-\mathbf u_i),\qquad\boxed{\boldsymbol\xi_i=\left(1-\frac{i\omega}{\mu}\right)\boldsymbol\xi_n,\quad\frac{\xi_n}{\xi_i}=\frac{\mu}{\mu-i\omega}.}
$$

The [vector](../../../../../../vector.md) [displacements](../../../../../../displacement.md) are parallel as complex polarization [vectors](../../../../../../vector.md), with this scalar amplitude and phase ratio.

For the rapidly damped root, $\mu-i\omega_d=-\mu+a^2/(4\mu)+O(a^4/\mu^3)$, and hence

$$
\boxed{\frac{\xi_n}{\xi_i}=-1-\frac{a^2}{4\mu^2}+O\left(\frac{a^4}{\mu^4}\right).}
$$

The two fluids move almost equally and oppositely; [collisions](../../../../../../collision.md) remove the counterflow at a rate close to $2\mu$.

For either weakly damped [Alfvén wave](../../../../../../alfven-wave.md), expand the ratio around unity:

$$
\boxed{\frac{\xi_n}{\xi_i}=1\pm i\frac{a}{\sqrt2\mu}+O\left(\frac{a^2}{\mu^2}\right).}
$$

Equivalently, the exact slippage relation is $\boldsymbol\xi_i-\boldsymbol\xi_n=-(i\omega/\mu)\boldsymbol\xi_n$. Thus the relative slippage has size $|a|/(\sqrt2\mu)\ll1$ and is primarily a small phase difference. The fluids almost share a common [displacement](../../../../../../displacement.md), but [magnetic tension](../../../../../../magnetic-tension.md) acts directly on the [ions](../../../../../../ion.md) and drag accelerates the neutrals. This imperfect locking causes [ambipolar damping](../../../../../../ambipolar-damping.md).

The sign of the damping is also checked by the perturbation [energy](../../../../../../energy.md) balance. With periodic or vanishing-flux boundaries,

$$
\frac{d}{dt}\int\left[\frac\rho2(|\mathbf u_i|^2+|\mathbf u_n|^2)+\frac{|\delta\mathbf B|^2}{8\pi}\right]dV=-\rho\mu\int|\mathbf u_i-\mathbf u_n|^2dV\leq0.
$$

It follows by dotting each linear momentum equation with its [velocity](../../../../../../velocity.md) and the induction equation with $\delta\mathbf B/(4\pi)$; magnetic-tension work cancels magnetic-energy change, [pressure](../../../../../../pressure.md) contributes only boundary flux, and the two drag terms combine into the negative square. Even though spatial diffusion was neglected, ion-neutral friction still dissipates the [wave](../../../../../../wave.md) [energy](../../../../../../energy.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
