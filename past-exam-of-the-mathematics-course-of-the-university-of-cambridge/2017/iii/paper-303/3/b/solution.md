<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compute the coupling flow at zero [magnetic field](../../../../../../magnetic-field.md), or assume the source has support only in retained [Fourier modes](../../../../../../fourier-mode.md), so that the shell [Gaussian measure](../../../../../../gaussian-measure.md) is centered. First justify the shell propagator. For a positive quadratic kernel on the shell, the [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) gives [covariance](../../../../../../covariance.md) equal to the inverse kernel,

$$
\langle\widetilde\phi_>(\mathbf p)\widetilde\phi_>(\mathbf q)\rangle_0^{\rm shell}=(2\pi)^D\delta^{(D)}(\mathbf p+\mathbf q)\frac{\alpha}{p^2+\alpha r_0},
$$

with both momenta restricted to $\Lambda/b<|\mathbf p|\leq\Lambda$. Inserting the [Fourier transforms](../../../../../../fourier-transform.md) and using the [Dirac delta function](../../../../../../dirac-delta-function.md) yields the [Gaussian shell covariance](../../../../../../gaussian-shell-covariance.md)

$$
\boxed{G_>(\mathbf x-\mathbf y)=\int_{\Lambda/b<|\mathbf p|\leq\Lambda}\frac{d^Dp}{(2\pi)^D}\frac{\alpha e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}}{p^2+\alpha r_0}.}
$$

Changing $\mathbf p$ to $-\mathbf p$ gives the negative-exponent convention as well. The dependence is on the separation, as required by [translation invariance](../../../../../../translation-invariance.md). The printed numerator uses $\mathbf x$ alone: it is correct only if that symbol means the separation or if $\mathbf y=0$. For example at $\mathbf x=\mathbf y\ne0$, the [covariance](../../../../../../covariance.md) must equal the constant coincident value $G_>(0)$, while the literal printed integral generally depends on $\mathbf x$. Thus the missing separation is a real source qualification, not a change of Fourier-sign convention.

Integrating out the shell gives $H_{\rm eff}[\phi_<]=H_0[\phi_<]-\log\langle e^{-V[\phi_<+\phi_>]}\rangle_0^{\rm shell}$, up to a field-independent constant. At first order in $u_0$, the [cumulant expansion of a coarse-grained free energy](../../../../../../cumulant-expansion-of-a-coarse-grained-free-energy.md) retains $\langle V\rangle$. Odd moments of the centered [Gaussian measure](../../../../../../gaussian-measure.md) vanish and [Wick theorem](../../../../../../wick-s-theorem.md) gives $\langle\phi_>^4\rangle=3G_>(0)^2$. Writing $I_1=G_>(0)$,

$$
\langle V\rangle=\frac{u_0}{24}\int d^Dx\,[\phi_<^4+6I_1\phi_<^2+3I_1^2].
$$

The last term affects only the constant; the second is a momentum-independent [tadpole diagram](../../../../../../tadpole-diagram.md) correction. Before rescaling it changes $r_0$ to $r_0+u_0I_1/2$, leaves the quartic coefficient at $u_0$, and produces no [gradient](../../../../../../gradient.md) correction. Combining with part (a) gives the leading coupling recursion

$$
\boxed{r_0'=b^2\left(r_0+\frac{u_0}{2}I_1\right)+O(u_0^2),\qquad u_0'=b^{4-D}u_0+O(u_0^2),\qquad \alpha^{-1\prime}=\alpha^{-1}+O(u_0^2).}
$$

This is [one-loop shell mass renormalization in scalar quartic theory](../../../../../../one-loop-shell-mass-renormalization-in-scalar-quartic-theory.md). Here $I_1=\int_{\rm shell}d^Dp\,(2\pi)^{-D}\alpha/(p^2+\alpha r_0)$. The shell Gaussian is well defined if $p^2+\alpha r_0>0$ there; near $r_0=0$ this follows from $\alpha>0$. A negative slow-mode mass may be stabilized by the retained quartic term and does not require pretending that the full unconstrained quadratic measure at negative mass is normalizable.

Linearizing about $(r_0,u_0)=(0,0)$ gives

$$
\begin{pmatrix}r_0'\\u_0'\end{pmatrix}=\begin{pmatrix}b^2&\tfrac12b^2I_1(0)\\0&b^{4-D}\end{pmatrix}\begin{pmatrix}r_0\\u_0\end{pmatrix}+O(r_0u_0,u_0^2).
$$

Its mass and quartic [eigenvalues](../../../../../../eigenvalue.md) are $b^2$ and $b^{4-D}$. The off-diagonal term is an additive critical-mass shift: setting the bare $r_0=0$ is not generally the critical tuning when $u_0>0$. The mass remains relevant for every $D$; at $D=2$ the two linear [eigenvalues](../../../../../../eigenvalue.md) coincide and the [matrix](../../../../../../matrix.md) can have a [Jordan block](../../../../../../jordan-block.md), but both perturbations are still relevant.

For $D>4$, the quartic interaction is an [irrelevant operator](../../../../../../irrelevant-operator.md), and the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md) attracts weak quartic perturbations after the mass and [magnetic field](../../../../../../magnetic-field.md) have been tuned. The quartic can nevertheless be a [dangerously irrelevant coupling](../../../../../../dangerously-irrelevant-coupling.md): its positive value stabilizes the ordered phase. For $D<4$, it is a [relevant operator](../../../../../../relevant-operator.md), so the Gaussian description is unstable toward interactions. At $D=4$ it is a [marginal operator](../../../../../../marginal-operator.md); first-order perturbation theory alone does not decide its fate.

To settle that borderline case, retain the leading quartic contribution from the second cumulant, at zero external momentum in the local expansion. The two-fast-field part of $V$ is $(u_0/4)\int\phi_<^2\phi_>^2$. Since $\langle\phi_>^2(\mathbf x)\phi_>^2(\mathbf y)\rangle_c=2G_>(\mathbf x-\mathbf y)^2$, its connected second cumulant contributes

$$
-\frac{u_0^2}{16}\int d^Dx\,d^Dy\,\phi_<^2(\mathbf x)\phi_<^2(\mathbf y)G_>(\mathbf x-\mathbf y)^2.
$$

Keeping the local quartic term and using [Parseval identity](../../../../../../parseval-identity.md) gives $\int d^Dy\,G_>(\mathbf x-\mathbf y)^2=I_2$, where $I_2=\int_{\rm shell}d^Dp\,(2\pi)^{-D}[\alpha/(p^2+\alpha r_0)]^2$. Thus the [one-loop shell quartic renormalization](../../../../../../one-loop-shell-quartic-renormalization.md) is

$$
\boxed{u_0'=b^{4-D}\left[u_0-\frac32u_0^2I_2\right]+\text{higher-order and derivative terms}.}
$$

The coefficient follows from multiplying the quartic density correction $-u_0^2I_2/16$ by $4!=24$. This local, zero-external-momentum coupling extraction is not a claim that the exact finite-shell effective action retains only its original [polynomial](../../../../../../polynomial-split.md); further operators are generated.

More explicitly, for a thin shell $b=e^{d\ell}$, let $c_D=\operatorname{area}(S^{D-1})/(2\pi)^D$, $R=\alpha r_0/\Lambda^2$ and $g=c_D\alpha^2\Lambda^{D-4}u_0$. With increasing length scale $\ell$, the leading flow is

$$
\frac{dR}{d\ell}=2R+\frac{g}{2(1+R)}+O(g^2),\qquad \frac{dg}{d\ell}=(4-D)g-\frac{3g^2}{2(1+R)^2}+O(g^3).
$$

This convention has the opposite scale direction to a [renormalization-group beta function](../../../../../../beta-function-physics.md) defined using increasing momentum. On the tuned [critical surface](../../../../../../critical-surface.md) at $D=4$, $R=O(g)$ and $dg/d\ell=-3g^2/2+O(g^3)$, so weak positive $g$ is [marginally irrelevant](../../../../../../marginally-irrelevant-operator.md), tending to zero with logarithmic corrections rather than remaining an exactly marginal parameter. Just below four dimensions, $D=4-\varepsilon$ with $0<\varepsilon\ll1$, the same calculation yields the [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) $g_*=2\varepsilon/3+O(\varepsilon^2)$, $R_*=-\varepsilon/6+O(\varepsilon^2)$. It does not justify extrapolating a small-$\varepsilon$ expansion to every lower dimension. The ordinary scalar quartic [upper critical dimension](../../../../../../upper-critical-dimension.md) is therefore

$$
\boxed{D_c=4.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
