<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the exact scalar-metric normalization specified by the preceding brightness equation:

$$
h_{ij}n^in^j=\frac h3+\left(\mu^2-\frac13\right)h_s.
$$

The [temperature](../../../../../../temperature.md) source is therefore $-(h'-h_s')/6-\mu^2h_s'/2$. Let $W=e^{ik\mu(\tau-\tau_0)}$, so $W'=ik\mu W$ and $W''=-k^2\mu^2W$. The formula just derived becomes

$$
\Theta_0=W_*\left(\frac{\delta_\gamma}4+\mathbf n\cdot\mathbf v\right)_*
-\int_{\tau_*}^{\tau_0}W\frac{h'-h_s'}6\,d\tau
-\frac{\mu^2}2\int_{\tau_*}^{\tau_0}Wh_s'\,d\tau.
$$

For $k\ne0$ the last term may be integrated twice by parts:

$$
\begin{aligned}
-\frac{\mu^2}2\int Wh_s'd\tau
&=\frac1{2k^2}\int W''h_s'd\tau\\
&=\frac1{2k^2}\left[W'h_s'-Wh_s''\right]_{\tau_*}^{\tau_0}
+\frac1{2k^2}\int Wh_s'''d\tau.
\end{aligned}
$$

No field equation beyond the supplied brightness relation has been used for this identity.

For scalar [velocity](../../../../../../velocity.md) the supplied [photon continuity equation](../../../../../../photon-continuity-equation.md) gives

$$
i\mathbf k\cdot\mathbf v=-\frac34\delta_\gamma'-\frac12h',
\qquad
\mathbf n\cdot\mathbf v=\frac{3i\mu}{4k}\delta_\gamma'
+\frac{i\mu}{2k}h'.
$$

The sign follows from division by $i$: with the Fourier streaming term $+ik\mu$, the [velocity](../../../../../../velocity.md) projection has the plus $h'$ term shown here. Combining it with the lower endpoint from the integrations by parts gives the complete [endpoint terms in the synchronous Sachs-Wolfe formula](../../../../../../endpoint-terms-in-the-synchronous-sachs-wolfe-formula.md):

$$
\boxed{\begin{aligned}
\Theta_0={}&W_*\left[
\frac14\delta_\gamma+\frac{3i\mu}{4k}\delta_\gamma'
+\frac{i\mu}{2k}(h'-h_s')+\frac{h_s''}{2k^2}\right]_*\\
&+\left[\frac{i\mu}{2k}h_s'-\frac{h_s''}{2k^2}\right]_0\\
&-\int_{\tau_*}^{\tau_0}W(\tau)
\left[\frac{h'-h_s'}6-\frac{h_s'''}{2k^2}\right]d\tau.
\end{aligned}}
$$

The local observer bracket is an angular [photon monopole](../../../../../../photon-monopole.md) plus [photon dipole](../../../../../../photon-dipole.md). Removing the local mean [temperature](../../../../../../temperature.md) and [photon dipole](../../../../../../photon-dipole.md), or restricting the result to measured multipoles $\ell\geq2$, permits omitting that bracket. It must be retained for the literal full brightness amplitude. The $k=0$ limit should be taken in the original line-of-sight integral, rather than treating the separate inverse-$k$ endpoint terms as independently defined.

**The final target formula printed in the PDF does not follow from its preceding equations.** With the stated streaming and scalar conventions, the decoupling terms proportional to $h'-h_s'$ and $h_s''$ have plus signs as derived above, not the printed minus signs. Moreover the integral has no additional outside factor $1/2$ when its bracket is $(h'-h_s')/6-h_s'''/(2k^2)$. Equivalently one may retain an outside $-1/2$ only if that bracket is doubled to $(h'-h_s')/3-h_s'''/k^2$. Omitting the observer [photon monopole](../../../../../../photon-monopole.md) and [photon dipole](../../../../../../photon-dipole.md) does not fix these discrepancies.

For a direct counterexample to the integral coefficient, take $h_s=0$, $h'=\varepsilon$ constant, $\mu=0$, and $\delta_{\gamma *}=\delta_{\gamma *}'=0$. A scalar emission [velocity](../../../../../../velocity.md) with $i\mathbf k\cdot\mathbf v_*=-\varepsilon/2$ satisfies the stated continuity equation; its projection along this transverse [photon](../../../../../../photon.md) direction is zero. Keep $\varepsilon(\tau_0-\tau_*)\ll1$ so [perturbation theory](../../../../../../perturbation-theory.md) is valid. The original brightness equation or the line-of-sight integral gives

$$
\Theta_0=-\frac{\varepsilon(\tau_0-\tau_*)}{6},
$$

whereas the printed final expression gives $-\varepsilon(\tau_0-\tau_*)/12$. All $h_s$ observer terms vanish in this example, so an observer-term convention cannot remove the contradiction. The boxed corrected identity supplies the requested integration-by-parts result with every boundary contribution and its observable higher-multipole version specified.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
