<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A=k^2v_A^2>0$ and $C=N^2+\Omega^2$. Solving the [radially stratified magnetorotational dispersion relation](../../../../../../radially-stratified-magnetorotational-dispersion-relation.md) as a quadratic in $s=\sigma^2$ gives

$$
s_\pm=-A-\frac C2\pm\frac12\sqrt{C^2+16\Omega^2A}.
$$

Both roots are real. If $A+N^2-3\Omega^2<0$, their product is negative, so exactly one root is positive and gives exponential growth. Conversely, when $A+N^2-3\Omega^2\geq0$, the coefficient $2A+N^2+\Omega^2\geq A+4\Omega^2>0$, so both roots are nonpositive. Thus **the instability criterion for a specified nonzero [wavenumber](../../../../../../wavenumber.md)** is

$$
\boxed{0<k^2v_A^2<3\Omega^2-N^2.}
$$

In a local continuum of allowed [wavenumbers](../../../../../../wavenumber.md), some unstable mode exists exactly when $N^2<3\Omega^2$. A finite disk only permits [wavelengths](../../../../../../wavelength.md) fitting its vertical boundaries, so this existence statement also requires an allowed mode in the interval.

The growing root is $s_+$, whose derivative and curvature are

$$
\frac{ds_+}{dA}=-1+\frac{4\Omega^2}{\sqrt{C^2+16\Omega^2A}},\qquad
\frac{d^2s_+}{dA^2}=-\frac{32\Omega^4}{(C^2+16\Omega^2A)^{3/2}}<0.
$$

Setting the derivative to zero gives **the fastest-growing interior mode**:

$$
\boxed{k_{\max}^2v_A^2=\Omega^2-\frac{(N^2+\Omega^2)^2}{16\Omega^2}.}
$$

For a real, nonzero [wavenumber](../../../../../../wavenumber.md), this expression requires $|N^2+\Omega^2|<4\Omega^2$, equivalently

$$
\boxed{-5\Omega^2<N^2<3\Omega^2.}
$$

Nonnegative right-hand side permits the endpoints, but there the stationary point is at $k=0$, outside the nonzero-[wavenumber](../../../../../../wavenumber.md) mode used above. Substituting the interior maximizing value gives

$$
s_{\max}=\frac{(3\Omega^2-N^2)^2}{16\Omega^2},\qquad\boxed{\sigma_{\max}=\frac{3\Omega^2-N^2}{4\Omega}.}
$$

This is the [maximum growth rate of radially stratified magnetorotational instability](../../../../../../maximum-growth-rate-of-radially-stratified-magnetorotational-instability.md), taking $\Omega>0$. For $N^2=0$ it reduces to the usual $3\Omega/4$, at $k^2v_A^2=15\Omega^2/16$. Negative $N^2$ enhances growth and extends the unstable band; positive $N^2$ suppresses growth and eventually eliminates it at $N^2\geq3\Omega^2$. [Magnetic tension](../../../../../../magnetic-tension.md) enables angular-momentum exchange between displaced parcels, weakening the rotational stabilization that protected the adverse hydrodynamic stratification.

If $N^2\leq-5\Omega^2$, the interior formula is no longer the physical maximum: $s_+$ decreases for $A>0$, and its supremum as $k\to0$ is $-N^2-\Omega^2$. The corresponding limiting growth rate is $\sqrt{-N^2-\Omega^2}$, dominated by the already unstable hydrodynamic branch. At $N^2=-5\Omega^2$ this joins continuously to $2\Omega$. For the smooth [thin disk](../../../../../../thin-disk.md) estimate $N^2\sim-(H/r)^2\Omega^2$, the ordinary interior maximum applies and its enhancement over $3\Omega/4$ is only of fractional order $(H/r)^2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
