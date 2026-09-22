<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\psi_0$ be the normalized stationary profile. Multiplying its stationary [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) by $\psi_0^*$, integrating and integrating the kinetic term by parts yields

$$
\boxed{\mu=\frac1N\int\left[\frac{\hbar^2}{2m}|\nabla\psi_0|^2+V_{\rm ext}|\psi_0|^2+U|\psi_0|^4\right]d^3x.}
$$

This is not simply $H/N$: the quartic contribution is twice its contribution to that energy per particle. For an infinite periodic system one uses one cell and the corresponding cell particle number, or equivalently average densities.

At fixed lattice spacing, mean density $n$, coupling and temperature, the commonly used [condensate compressibility in an optical lattice](../../../../../../condensate-compressibility-in-an-optical-lattice.md) is

$$
\boxed{\kappa^{-1}=n\left(\frac{\partial\mu}{\partial n}\right)_s.}
$$

If [compressibility](../../../../../../compressibility.md) means the thermodynamic volume response instead, the [Gibbs-Duhem equation](../../../../../../gibbs-duhem-equation.md) $dp=n\,d\mu$ at zero temperature gives $\kappa_T=[n^2(\partial\mu/\partial n)_s]^{-1}=\kappa/n$. Stating the convention removes this factor-of-density ambiguity; the lattice-depth derivative has the same sign at fixed $n$.

For the stable repulsive ground-band [Bose-Einstein condensate](../../../../../../bose-einstein-condensate.md), the intended trend is **$\partial\kappa/\partial s<0$ for increasing nonzero lattice depth**, with mean density held fixed. Deeper wells localize the field, enhancing the repulsive interaction response. To quantify this, in the weak-interaction band approximation write $\psi_0=\sqrt n f_s$, with the cell average of $|f_s|^2$ equal to one. Perturbation in $Un$ gives

$$
\mu=E_0(s)+Un I(s)+\cdots,\qquad
I(s)=\frac1d\int_0^d|f_s|^4dx,\qquad \kappa\simeq\frac1{UnI(s)}.
$$

In deep wells the localized orbital is approximately a normalized Gaussian of width $a_{\rm ho}=d/(\pi s^{1/4})$. Neglecting interwell overlap, $I\simeq d/(\sqrt{2\pi}a_{\rm ho})=\sqrt{\pi/2}\,s^{1/4}$, hence $\partial\kappa/\partial s\simeq-\kappa/(4s)<0$. This explicitly establishes the sign in that controlled regime; [the repulsive ground-band calculation](https://arxiv.org/abs/cond-mat/0305300) describes the broader trend.

The sign statement needs the repulsive, stable ground-band interpretation, not merely the literal assumption $U\ne0$. It also need not be a strictly nonzero derivative at $s=0$: at weak interaction $f_s=1+(s/8)\cos(2\pi x/d)+O(s^2)$, with normalization corrected at second order, gives $I=1+s^2/32+O(s^3)$ and a zero initial slope. A leading density-dominated [Thomas–Fermi approximation for a condensate](../../../../../../thomas-fermi-approximation-for-a-condensate.md) with density positive everywhere gives $\mu=Un+sE_R/2$ and no depth dependence of this response at that approximation's order. These limits do not justify a strict universal sign for every unspecified interaction and parameter regime.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
