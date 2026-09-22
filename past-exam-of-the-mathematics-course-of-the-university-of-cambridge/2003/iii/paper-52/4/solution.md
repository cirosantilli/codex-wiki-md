<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [instanton](../../../../../instanton.md) is a localized finite-action classical solution of a Euclidean field theory. Its role differs from that of a static spatial [classical field-theory soliton](../../../../../classical-field-theory-soliton-split.md): an instanton is localized in Euclidean spacetime and contributes to quantum transition amplitudes, rather than persisting as a stationary real-time particle. [Wick rotation](../../../../../wick-rotation.md) changes the oscillatory weight $e^{iS/\hbar}$ into $e^{-S_E/\hbar}$ when the continuation and boundary conditions are valid. The [Euclidean path integral](../../../../../euclidean-path-integral.md) is consequently dominated semiclassically by stationary Euclidean configurations. Perturbation theory around one vacuum misses other saddles whose weights have the nonanalytic form $e^{-S_I/\hbar}$.

A useful first example is [quantum tunnelling](../../../../../quantum-tunnelling.md) between two degenerate minima in quantum mechanics. For coordinate $q$ with mass $m$, the [Euclidean action](../../../../../euclidean-action.md) is

$$
S_E[q]=\int\left[\frac m2\dot q^2+V(q)\right]d\tau,
$$

with the vacuum energy subtracted from $V$. Its Euler-Lagrange equation is $m\ddot q=V'(q)$, equivalent to motion in the inverted potential $-V$. A finite-action trajectory joining zero-energy minima has conserved Euclidean energy $m\dot q^2/2-V=0$. A forward instanton therefore satisfies $\dot q=\sqrt{2V/m}$, while an [anti-instanton](../../../../../anti-instanton.md) has the opposite orientation. Completing the square gives the action bound

$$
S_E\ge\left|\int_{q_-}^{q_+}\sqrt{2mV(q)}\,dq\right|,
$$

which these zero-energy paths saturate. This is the Euclidean counterpart of the first-order kink argument, with Euclidean time replacing the spatial coordinate.

For the [quartic double-well instanton](../../../../../quartic-double-well-instanton.md), choose

$$
V(q)=\frac{m\omega^2}{8a^2}(q^2-a^2)^2.
$$

The first-order equation in the interval $-a<q<a$ is $\dot q=\omega(a^2-q^2)/(2a)$. Separation gives

$$
\boxed{q_I(\tau)=a\tanh\left[\frac{\omega(\tau-\tau_0)}2\right],\qquad S_I=\int_{-a}^a\sqrt{2mV}\,dq=\frac{2m\omega a^2}{3}.}
$$

The center $\tau_0$ is arbitrary. Its derivative $\dot q_I$ is an [instanton translation zero mode](../../../../../instanton-translation-zero-mode.md): differentiating the Euclidean field equation shows that it lies in the kernel of the quadratic fluctuation operator $-m\partial_\tau^2+V''(q_I)$. A naive Gaussian determinant therefore has a zero eigenvalue. Replace its integration by the collective-coordinate integral over $\tau_0$, and take the determinant only over nonzero modes. The resulting [instanton fluctuation prefactor](../../../../../instanton-fluctuation-prefactor.md) combines that Jacobian with the determinant ratio against the vacuum. The action controls the exponential suppression; the prefactor is essential for a quantitative rate or splitting.

When $S_I/\hbar\gg1$, crossings are rare and their typical separations greatly exceed their widths. In the [dilute instanton gas](../../../../../dilute-instanton-gas.md), ordered center integrals for $n$ well-separated crossings over Euclidean duration $\mathcal T$ produce $\mathcal T^n/n!$. If a single-crossing rate is $\kappa=K e^{-S_I/\hbar}$, a symmetric two-well system has even-crossing and odd-crossing sums proportional to $\cosh(\kappa\mathcal T)$ and $\sinh(\kappa\mathcal T)$. The spectral interpretation gives levels $E_{\rm well}\mp\hbar\kappa$ and

$$
\boxed{\Delta E=2\hbar K e^{-S_I/\hbar}.}
$$

This is a real tunnelling level splitting. A [Euclidean bounce](../../../../../euclidean-bounce.md) instead describes [false vacuum](../../../../../false-vacuum.md) decay: it leaves and returns to a metastable vacuum, and a characteristic negative fluctuation mode supplies the imaginary part interpreted as decay. A bounce must not be confused with a stable double-well instanton merely because both use Euclidean saddles.

The central gauge-theory example is a [Yang-Mills instanton](../../../../../yang-mills-instanton.md) on Euclidean four-space. State conventions carefully: take anti-Hermitian generators $T_a=-i\sigma_a/2$, with $\operatorname{Tr}(T_aT_b)=-\delta_{ab}/2$, connection $A=A_\mu dx^\mu$, and [gauge curvature](../../../../../gauge-field-strength.md) $F=dA+A\wedge A$. With coupling $g$, the positive [Yang-Mills action](../../../../../yang-mills-action.md) is

$$
S_E=-\frac1{g^2}\int\operatorname{Tr}(F\wedge *F)=\frac1{4g^2}\int F^a_{\mu\nu}F^a_{\mu\nu}\,d^4x.
$$

The [Hodge star operator](../../../../../hodge-star-operator.md) squares to one on Euclidean two-forms. Under the usual finite-action boundary conditions, the connection approaches a pure gauge at infinity, defining a map $S^3_\infty\to SU(2)\simeq S^3$. Its winding degree is the integer [instanton number](../../../../../instanton-number.md)

$$
k=-\frac1{8\pi^2}\int\operatorname{Tr}(F\wedge F)\in\mathbb Z.
$$

This is unchanged by smooth deformations preserving the boundary sector. Geometrically this is, up to the stated sign convention, the second Chern number of the compactified bundle. Different sign conventions for trace, curvature or orientation must be changed together.

Use the positive norm $\|F\|^2=-\int\operatorname{Tr}(F\wedge *F)$. Decomposition into self-dual and anti-self-dual curvature gives

$$
S_E=\frac1{2g^2}\|F\mp *F\|^2\pm\frac{8\pi^2k}{g^2}\ge\frac{8\pi^2|k|}{g^2}.
$$

The [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md) is saturated by $F=*F$ for positive $k$, or $F=-*F$ for negative $k$. These first-order equations imply the full [Yang-Mills equations](../../../../../yang-mills-equations.md): the [Bianchi identity](../../../../../bianchi-identity.md) $D_AF=0$ becomes $D_A*F=0$ when $*F=\pm F$. Thus the topological minimum is a genuine classical saddle, not just an arbitrary field with integer charge. Self-duality alone is a local differential condition; finite action is an additional requirement.

An explicit unit-charge example is the [BPST instanton](../../../../../bpst-instanton.md). Let $y=x-x_0$, $\rho>0$, and choose the self-dual symbols $\eta^a_{ij}=\epsilon_{aij}$, $\eta^a_{i4}=\delta_{ai}$ and $\eta^a_{4i}=-\delta_{ai}$ for $i,j=1,2,3$, using orientation $dx^1\wedge dx^2\wedge dx^3\wedge dx^4$. In regular gauge,

$$
A_\mu=\frac{2\eta^a_{\mu\nu}y^\nu}{y^2+\rho^2}T_a,\qquad F_{\mu\nu}=-\frac{4\rho^2\eta^a_{\mu\nu}}{(y^2+\rho^2)^2}T_a.
$$

The curvature is self-dual. Since $\sum_{a,\mu,\nu}(\eta^a_{\mu\nu})^2=12$, its squared component curvature is $192\rho^4/(y^2+\rho^2)^4$. Radial integration yields

$$
S_E=\frac{48\rho^4}{g^2}\,2\pi^2\int_0^\infty\frac{r^3}{(r^2+\rho^2)^4}\,dr=\frac{8\pi^2}{g^2},
$$

so $k=1$. Replacing self-dual symbols by anti-self-dual ones produces the opposite charge with the same positive action.

The center has four coordinates and $\rho$ is an [instanton size modulus](../../../../../instanton-size-modulus.md). Classical four-dimensional Yang-Mills action is scale invariant, so varying $\rho$ changes the action-density width but not the total action. If gauge transformations must tend to the identity at infinity, three global gauge orientations also remain, giving eight parameters for the one-instanton [framed instanton moduli space](../../../../../framed-instanton-moduli-space.md). If those global orientations are quotiented out, the unframed one-instanton space has five parameters. A zero-size limit is a singular concentration of curvature, not another smooth instanton. Higher-charge solutions likewise possess [instanton moduli spaces](../../../../../instanton-moduli-space.md); their collective-coordinate integrals replace the corresponding zero-mode determinants.

In a Euclidean-time description, topologically distinct gauge vacua are separated by a change of [Chern-Simons number](../../../../../chern-simons-number-of-a-gauge-field.md); an instanton interpolates between them, with the change equal to $k$ in compatible orientation conventions. [Theta-weighted instanton sectors](../../../../../theta-weighted-instanton-sectors.md) give $Z(\vartheta)=\sum_k e^{ik\vartheta}Z_k$, connecting topology to the vacuum angle. With fermions, the gauge-field topology also controls fermionic zero modes and chiral selection rules through the [chiral anomaly](../../../../../chiral-anomaly.md). These phenomena explain why instantons encode physics beyond small fluctuations around a single vacuum.

**Instantons link Euclidean classical solutions, topological sectors and exponentially suppressed quantum effects.** Their interpretation requires the boundary conditions, normalization, fluctuation spectrum and measure over collective coordinates. A dilute approximation is controlled only when its individual-action suppression and separation assumptions hold; classical scale moduli and their quantum corrections can make size integrals delicate rather than automatically finite.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
