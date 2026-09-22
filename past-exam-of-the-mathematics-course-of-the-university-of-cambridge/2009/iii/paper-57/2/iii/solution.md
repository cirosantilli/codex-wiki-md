<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the regular growing matter mode $\delta_c=C\tau^2$ and $h=-2C\tau^2$. With $\mathcal H=2/\tau$, the constraint gives

$$
-8C+\frac{k^2}{3}h^-=12C,\qquad h^-=\frac{60C}{k^2}.
$$

Consequently

$$
\zeta=\frac16h^-+\frac13\delta_c=\frac{10C}{k^2}+\frac13C\tau^2
=\zeta_*\left[1+\frac{(k\tau)^2}{30}\right].
$$

Here $\zeta_*=10C/k^2$ is its early, superhorizon constant value. The fractional time variation is of second gradient order, and

$$
\frac{\zeta'}{\mathcal H\zeta}=\frac{(k\tau)^2/30}{1+(k\tau)^2/30}\ll1.
$$

Thus **the primordial curvature is conserved to leading order on [superhorizon scales](../../../../../../superhorizon-scale.md)**. This is the [matter-era density transfer from primordial curvature](../../../../../../matter-era-density-transfer-from-primordial-curvature.md).

A mode entering after equality evolves in the growing matter solution, giving

$$
\boxed{\delta_c(k,\tau_0)=\frac{k^2\tau_0^2}{10}\zeta_*(k),\qquad
T_\delta(k)=\frac{k^2\tau_0^2}{10}\quad(k\ll k_{\rm eq}).}
$$

This assumes matter-dominated growth to $\tau_0$, as in the model. A subsequent dark-energy era would multiply by the appropriate late-time growth suppression. The initial radiation-era adiabatic curvature passes through equality unchanged at leading superhorizon order, so the same $\zeta_*$ is the primordial input.

For $k\gg k_{\rm eq}$, entry occurs in [radiation domination](../../../../../../radiation-domination.md) at $\tau_h\sim k^{-1}$. The entry contrast is of order $\zeta_*$ because its superhorizon value scales as $k^2\tau_h^2\zeta_*$. In the question's stagnation approximation it stays of this order until equality, then grows by $(\tau_0/\tau_{\rm eq})^2$. Thus

$$
\boxed{T_\delta(k)\sim\left(\frac{\tau_0}{\tau_{\rm eq}}\right)^2\quad(k\gg k_{\rm eq}),}
$$

independent of $k$ to that approximation. The precise coefficient needs matching through the equality transition; the horizon convention, including the use of wavelength $2\pi/k$, also changes the matching definition of $k_{\rm eq}\sim\tau_{\rm eq}^{-1}$ by a fixed factor.

One continuous sharp-equality model, normalizing the plateau by matching the low-$k$ branch at $k_{\rm eq}$, is the [sharp-equality cold-dark-matter transfer approximation](../../../../../../sharp-equality-cold-dark-matter-transfer-approximation.md)

$$
T_\delta(k)\simeq\frac{\tau_0^2}{10}\begin{cases}k^2,&k\leq k_{\rm eq},\\k_{\rm eq}^2,&k\geq k_{\rm eq}.\end{cases}
$$

This is a matching approximation, not an exact solution through equality. The function requested here transfers curvature directly to density. It differs from the conventional normalized matter transfer $\mathcal T(k)$, where one factors out $k^2\tau_0^2/10$: that normalized function tends to one at low $k$ and to $(k_{\rm eq}/k)^2$ in the stagnation model at high $k$.

For the dimensional primordial spectrum $P_\zeta=A/k^3$, linear deterministic transfer gives $P_c=|T_\delta|^2P_\zeta$. Hence this sharp model yields

$$
\boxed{P_c(k,\tau_0)\simeq\frac{A\tau_0^4}{100}\begin{cases}k,&k\ll k_{\rm eq},\\k_{\rm eq}^4/k^3,&k\gg k_{\rm eq}.\end{cases}}
$$

The spectrum turns over near equality. Retaining the slow radiation-era logarithmic growth refines the high-$k$ transfer to $T_\delta\propto(\tau_0/\tau_{\rm eq})^2\ln(k/k_{\rm eq})$, up to constants in the logarithm and matching factors, and therefore refines the small-scale spectrum to $P_c\propto k^{-3}\ln^2(k/k_{\rm eq})$. This is the [logarithmic small-scale matter transfer](../../../../../../logarithmic-small-scale-matter-transfer.md) correction to the question's constant-growth idealization. Multiplication by $k^3/(2\pi^2)$ would give dimensionless power, whose large-scale slope is $k^4$ rather than the dimensional spectrum's $k$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
