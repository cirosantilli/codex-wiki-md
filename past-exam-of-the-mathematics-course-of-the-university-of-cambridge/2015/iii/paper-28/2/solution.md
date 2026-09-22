<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A normalization is important here. I use the [covolume-one theta function of a fractional ideal](../../../../../covolume-one-theta-function-of-a-fractional-ideal.md), for which the requested limit is $1$, and also give the formula for the unnormalized [Gaussian theta sum](../../../../../gaussian-theta-sum.md).

Let $n=[K:\mathbb Q]$, let $d_v=[K_v:\mathbb R]\in\{1,2\}$, and choose one [field embedding](../../../../../field-embedding.md) $\sigma_v$ for each [Archimedean place](../../../../../archimedean-place.md). The [Minkowski embedding of a number field](../../../../../minkowski-embedding-of-a-number-field.md) identifies

$$
K_\infty=\mathbb R^{r_1}\times\mathbb C^{r_2},\qquad n=r_1+2r_2,
$$

with a real [inner product space](../../../../../inner-product-space.md) having

$$
\langle x,z\rangle=\sum_{v\text{ real}}x_vz_v+2\sum_{v\text{ complex}}\operatorname{Re}(x_v\overline{z_v}),\qquad |x|^2=\sum_vd_v|x_v|^2.
$$

Its Euclidean [Lebesgue measure](../../../../../lebesgue-measure.md) is $d\mu=\prod_{v\text{ real}}dx_v\prod_{v\text{ complex}}2\,d\operatorname{Re}x_v\,d\operatorname{Im}x_v$. With this convention, the [covolume of a fractional ideal lattice](../../../../../covolume-of-a-fractional-ideal-lattice.md) $j(\mathfrak b)$ is

$$
C_{\mathfrak b}=\sqrt{|D_K|}\,N(\mathfrak b),
$$

where $D_K$ is the [field discriminant](../../../../../field-discriminant.md) and $N(\mathfrak b)$ is the positive absolute [norm of a fractional ideal](../../../../../norm-of-a-fractional-ideal.md). Thus the [Euclidean lattice](../../../../../euclidean-lattice.md) $\Lambda_{\mathfrak b}=C_{\mathfrak b}^{-1/n}j(\mathfrak b)$ has [covolume](../../../../../covolume.md) $1$. Define

$$
\boxed{\Theta(y,\mathfrak b)=\sum_{a\in\mathfrak b}\exp\left(-\pi C_{\mathfrak b}^{-2/n}\sum_{v\in S_\infty}d_vy_v|\sigma_v(a)|^2\right).}
$$

This [Gaussian theta sum](../../../../../gaussian-theta-sum.md) converges absolutely whenever every $y_v>0$.

The [trace dual of a fractional ideal](../../../../../trace-dual-of-a-fractional-ideal.md) is

$$
\mathfrak b^\vee=\mathfrak D_{K/\mathbb Q}^{-1}\mathfrak b^{-1}=\{z\in K:\operatorname{Tr}_{K/\mathbb Q}(z\mathfrak b)\subseteq\mathbb Z\}.
$$

Here $\mathfrak D_{K/\mathbb Q}^{-1}$ is the [inverse different](../../../../../inverse-different.md). Since $N(\mathfrak D_{K/\mathbb Q})=|D_K|$, we have $C_{\mathfrak b^\vee}=C_{\mathfrak b}^{-1}$. There is a subtle distinction between the [trace pairing](../../../../../trace-pairing.md) and the positive [inner product](../../../../../inner-product.md): the [dual lattice](../../../../../dual-lattice.md) of $j(\mathfrak b)$ is $\overline{j(\mathfrak b^\vee)}$, where the bar conjugates the complex coordinates and fixes the real ones. Indeed,

$$
\langle j(a),\overline{j(z)}\rangle=\operatorname{Tr}_{K/\mathbb Q}(az).
$$

Consequently $\Lambda_{\mathfrak b}^*=\overline{\Lambda_{\mathfrak b^\vee}}$. Coordinatewise [complex conjugation](../../../../../complex-conjugation.md) preserves the weighted squared lengths in the [Gaussian theta sum](../../../../../gaussian-theta-sum.md).

Here are the precise analytic formulas used in the proof. For a [Schwartz function](../../../../../schwartz-function.md) on $K_\infty$, take the [Fourier transform](../../../../../fourier-transform.md) to be

$$
\widehat f(z)=\int_{K_\infty}f(x)e^{-2\pi i\langle x,z\rangle}\,d\mu(x).
$$

For a full [Euclidean lattice](../../../../../euclidean-lattice.md) $\Lambda$ of [covolume](../../../../../covolume.md) $C$, the [Poisson summation formula for a Euclidean lattice](../../../../../poisson-summation-formula-for-a-euclidean-lattice.md) is

$$
\sum_{x\in\Lambda}f(x)=C^{-1}\sum_{z\in\Lambda^*}\widehat f(z).
$$

For $f_y(x)=\exp(-\pi\sum_vd_vy_v|x_v|^2)$, the [Gaussian Fourier transform](../../../../../fourier-transform-of-a-gaussian.md), applied in orthonormal real coordinates, gives

$$
\widehat f_y(z)=\|y\|^{-1/2}\exp\left(-\pi\sum_vd_vy_v^{-1}|z_v|^2\right),\qquad \|y\|=\prod_vy_v^{d_v}.
$$

More generally, $\widehat{\exp(-\pi x^TAx)}(z)=(\det A)^{-1/2}\exp(-\pi z^TA^{-1}z)$ for a real [positive-definite matrix](../../../../../positive-definite-matrix.md) $A$ that is symmetric. Each complex coordinate contributes two real coordinates, which explains its exponent $d_v=2$.

Apply the [Poisson summation formula for a Euclidean lattice](../../../../../poisson-summation-formula-for-a-euclidean-lattice.md) to $\Lambda_{\mathfrak b}$, whose [covolume](../../../../../covolume.md) is $1$, and use the preceding description of its [dual lattice](../../../../../dual-lattice.md). The [anisotropic theta functional equation](../../../../../anisotropic-theta-functional-equation.md) is

$$
\boxed{\Theta(y,\mathfrak b)=\|y\|^{-1/2}\Theta(y^{-1},\mathfrak b^\vee),\qquad (y^{-1})_v=y_v^{-1}.}
$$

For comparison, the unnormalized [Gaussian theta sum](../../../../../gaussian-theta-sum.md)

$$
\theta(y,\mathfrak b)=\sum_{a\in\mathfrak b}\exp\left(-\pi\sum_vd_vy_v|\sigma_v(a)|^2\right)
$$

has the [functional equation](../../../../../functional-equation.md)

$$
\theta(y,\mathfrak b)=C_{\mathfrak b}^{-1}\|y\|^{-1/2}\theta(y^{-1},\mathfrak b^\vee),
$$

and its corresponding limit is $C_{\mathfrak b}^{-1}$ rather than $1$. Explicitly, our normalization is $\Theta(y,\mathfrak b)=\theta(C_{\mathfrak b}^{-2/n}y,\mathfrak b)$.

For the [small-parameter asymptotic of a lattice theta sum](../../../../../small-parameter-asymptotic-of-a-lattice-theta-sum.md), $y\to0$ means that every coordinate tends to zero. In $\Theta(y^{-1},\mathfrak b^\vee)$, the zero lattice vector contributes $1$. Every nonzero vector contributes a term tending to zero. Once every $y_v\leq1$, all these terms are bounded by the summable [Gaussian theta sum](../../../../../gaussian-theta-sum.md) $\sum_{\lambda\in\Lambda_{\mathfrak b^\vee}}e^{-\pi|\lambda|^2}$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore gives $\Theta(y^{-1},\mathfrak b^\vee)\to1$. Using the [anisotropic theta functional equation](../../../../../anisotropic-theta-functional-equation.md),

$$
\boxed{\lim_{y\to0}\|y\|^{1/2}\Theta(y,\mathfrak b)=1.}
$$

The condition that every coordinate tends to zero matters; $\|y\|\to0$ alone would not justify this argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
