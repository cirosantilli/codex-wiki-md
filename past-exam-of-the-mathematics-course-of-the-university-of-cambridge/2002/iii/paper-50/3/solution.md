<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $\mu=\mu^0$, $\lambda=\kappa^0-2\mu/3$, and $L=\lambda+2\mu=\kappa^0+4\mu/3$. Assume positive [bulk modulus](../../../../../bulk-modulus.md) and [shear modulus](../../../../../shear-modulus.md). For a unit vector $\xi$, direct contraction of the isotropic [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) gives the [acoustic tensor](../../../../../acoustic-tensor.md) and its inverse:

$$
K(\xi)=\mu I+(L-\mu)\xi\otimes\xi,
\qquad K^{-1}(\xi)=\frac1\mu(I-\xi\otimes\xi)+\frac1L\xi\otimes\xi.
$$

These are its transverse and longitudinal [orthogonal projections](../../../../../orthogonal-projection.md). Symmetrizing the definition of the [directional elastic strain Green operator](../../../../../directional-elastic-strain-green-operator.md) consequently gives

$$
\widetilde\Gamma_{ijkl}(\xi)
=\frac1{4\mu}\bigl(\delta_{jk}\xi_i\xi_l+\delta_{ik}\xi_j\xi_l+\delta_{jl}\xi_i\xi_k+\delta_{il}\xi_j\xi_k\bigr)
+\left(\frac1L-\frac1\mu\right)\xi_i\xi_j\xi_k\xi_l.
$$

Substitution into the spherical representation is already the isotropic specialization. We can also evaluate its angular integrals as [distributions](../../../../../distribution-mathematical-analysis.md). For $r=|x|>0$, direct integration with the polar axis parallel to $x$ gives

$$
\int_{S^2}\delta(\xi\cdot x)\,dS=\frac{2\pi}{r},
\qquad\int_{S^2}|\xi\cdot x|\,dS=2\pi r.
$$

The first identity holds as a locally integrable [distribution](../../../../../distribution-mathematical-analysis.md). Since the second derivative of $|s|$ is $2\delta(s)$, taking two derivatives in the first identity and four in the second gives

$$
\int_{S^2}\xi_i\xi_j\delta''(\xi\cdot x)\,dS=2\pi\partial_i\partial_j(r^{-1}),
\qquad
\int_{S^2}\xi_i\xi_j\xi_k\xi_l\delta''(\xi\cdot x)\,dS=\pi\partial_i\partial_j\partial_k\partial_l r.
$$

Thus an explicit complete [isotropic elastic strain Green kernel](../../../../../isotropic-elastic-strain-green-kernel.md) is

$$
\begin{aligned}
\Gamma_{ijkl}(x)
={}&-\frac1{16\pi\mu}\bigl(\delta_{jk}\partial_i\partial_l+\delta_{ik}\partial_j\partial_l+\delta_{jl}\partial_i\partial_k+\delta_{il}\partial_j\partial_k\bigr)r^{-1}\\
&-\frac1{8\pi}\left(\frac1L-\frac1\mu\right)\partial_i\partial_j\partial_k\partial_l r.
\end{aligned}
$$

All derivatives here are [distributional derivatives](../../../../../distributional-derivative.md), which retain the contribution at the origin.

For the requested contraction, $\widetilde\Gamma_{ijkk}=\xi_i\xi_j/L$, or equivalently trace the complete kernel and use $\Delta r=2/r$. Therefore

$$
\boxed{\Gamma_{ijkk}(x)=-\frac1{4\pi L}\partial_i\partial_j\frac1{|x|}.}
$$

More explicitly, its [distribution](../../../../../distribution-mathematical-analysis.md) form is

$$
\Gamma_{ijkk}
=\frac{\delta_{ij}}{3L}\delta(x)
+\frac1{4\pi L}\operatorname{pv}\frac{\delta_{ij}|x|^2-3x_i x_j}{|x|^5},
$$

where the [Cauchy principal value](../../../../../cauchy-principal-value.md) uses spherical exclusions about the origin. The coefficient of the [Dirac delta](../../../../../dirac-delta-function.md) can be checked by integrating by parts over a punctured ball: $\partial_i\partial_j(r^{-1})$ has contact term $-4\pi\delta_{ij}\delta/3$. Taking the trace, the principal-value part has zero trace and $\Delta(r^{-1})=-4\pi\delta$, so

$$
\boxed{\Gamma_{iikk}(x)=\frac1L\delta(x).}
$$

Keeping only the ordinary kernel away from the origin would incorrectly give zero for this double trace.

Now extend the [elastic polarization](../../../../../elastic-polarization.md) by zero outside $V$. Since the [shear modulus](../../../../../shear-modulus.md) is unchanged, the stiffness contrast acts only on the spherical [strain](../../../../../strain.md):

$$
\tau_{ij}(x)=(C-C^0)_{ijkl}\varepsilon_{kl}(x)
=\bigl(\kappa(x)-\kappa^0\bigr)\varepsilon_{kk}(x)\delta_{ij}.
$$

Hence $\tau=(\kappa-\kappa^0)\operatorname{tr}\varepsilon$ is its scalar coefficient. Relative to the same external loading, the [elastic strain Green operator](../../../../../elastic-strain-green-operator.md) gives $\varepsilon=\varepsilon^0-\Gamma*(\tau I)$. Taking the trace and using the contact identity reduces this nonlocal equation to

$$
\varepsilon_{kk}(x)=\varepsilon^0_{kk}(x)-\frac{\kappa(x)-\kappa^0}{L}\varepsilon_{kk}(x).
$$

Solving the scalar equation gives the [constant-shear bulk-modulus inclusion](../../../../../constant-shear-bulk-modulus-inclusion.md) formula

$$
\boxed{\varepsilon_{kk}(x)=\frac{3\kappa^0+4\mu^0}{3\kappa(x)+4\mu^0}\varepsilon^0_{kk}(x).}
$$

Using the single contraction instead of the double trace gives

$$
\varepsilon_{ij}(x)=\varepsilon^0_{ij}(x)+\frac1{4\pi L}\partial_i\partial_j
\int_V\frac{(\kappa(x')-\kappa^0)\varepsilon_{kk}(x')}{|x-x'|}\,dx'.
$$

Finally eliminate the actual trace using the scalar formula:

$$
\boxed{\varepsilon_{ij}(x)=\varepsilon^0_{ij}(x)+\frac1{4\pi}\partial_i\partial_j
\int_V\frac{3(\kappa(x')-\kappa^0)}{3\kappa(x')+4\mu^0}
\frac{\varepsilon^0_{kk}(x')}{|x-x'|}\,dx'.}
$$

The reference trace $\varepsilon^0_{kk}$ in this last formula is essential and is what the original PDF prints; the converted TeX loses its superscript. The second derivatives are interpreted distributionally, or with their principal-value and contact terms explicitly included. With ordinary regularity they give the corresponding pointwise formula at regular interior points.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
