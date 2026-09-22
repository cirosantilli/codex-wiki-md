<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The opposite sign is the [focusing semilinear wave equation](../../../../../../focusing-semilinear-wave-equation.md) $\phi_{tt}-\Delta\phi=\phi^3$. Begin with a spatially constant solution, reducing the [partial differential equation](../../../../../../partial-differential-equation-split.md) to the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) $a''=a^3$. Substitution of $a(t)=\beta(t-1)^{-\alpha}$ gives

$$
\alpha(\alpha+1)\beta(t-1)^{-\alpha-2}=\beta^3(t-1)^{-3\alpha}.
$$

For a nonzero profile, equality of powers and coefficients gives $\alpha=1$ and $\beta^2=2$. Choose

$$
a(t)=\frac{\sqrt2}{1-t},\qquad a(0)=a'(0)=\sqrt2.
$$

To obtain [compact support](../../../../../../compact-support.md), take a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\chi$ equal to one on $B(0,2)$ and zero outside $B(0,3)$, and prescribe

$$
\phi_0=\sqrt2\chi,\qquad\phi_1=\sqrt2\chi.
$$

These are smooth, compactly supported [Cauchy data](../../../../../../cauchy-data.md). By [finite propagation speed](../../../../../../finite-propagation-speed.md), the local solution agrees with $a(t)$ throughout $|x|<2-t$ for $0\leq t<\min(1,T_*)$, where $T_*$ is its maximal forward smooth existence time.

For completeness, the semilinear [domain of dependence](../../../../../../domain-of-dependence.md) assertion follows by comparing two solutions: their difference $z$ obeys $z_{tt}-\Delta z=bz$, with $b=\phi^2+\phi a+a^2$. On any compact time interval before $t=1$ on which the solutions are smooth, $b$ is bounded in the backward [light cone](../../../../../../light-cone.md). Add $z^2/2$ to the shrinking-ball [wave energy](../../../../../../wave-energy.md); its derivative is bounded above by $C$ times that energy, with the same nonpositive boundary flux. Zero initial difference and the [Gronwall inequality](../../../../../../gronwall-inequality.md) give $z=0$ there.

If $T_*>1$, the identity at the origin would imply $\phi(t,0)=\sqrt2/(1-t)$ as $t\uparrow1$, contradicting smoothness at $t=1$. Thus

$$
\boxed{T_*\leq1<\infty.}
$$

If the solution loses regularity earlier, that is already finite-time blowup. The usual [smooth continuation criterion for semilinear wave equations](../../../../../../smooth-continuation-criterion-for-semilinear-wave-equations.md) precludes a finite maximal time with all continuation norms bounded. This [localized ordinary differential equation blowup for a wave equation](../../../../../../localized-ordinary-differential-equation-blowup-for-a-wave-equation.md) therefore supplies the required compactly supported examples.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
