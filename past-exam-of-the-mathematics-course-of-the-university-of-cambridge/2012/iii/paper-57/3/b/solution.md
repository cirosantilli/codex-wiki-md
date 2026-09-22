<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a statistically homogeneous isotropic dimensionless field, write its two-point [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md) as $C(r)$ and

$$
C(r)=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
$$

The formal real-space [scale invariance](../../../../../../scale-invariance.md) condition is $C(\lambda\mathbf r)=C(\mathbf r)$ for all $\lambda>0$. Changing variable $\mathbf q=\lambda\mathbf k$ in the first expression and equating the nonzero-mode [Fourier transforms](../../../../../../fourier-transform.md) gives $\lambda^{-3}P(q/\lambda)=P(q)$, equivalently $P(\lambda k)=\lambda^{-3}P(k)$. Taking $\lambda=k/k_0$ yields

$$
\boxed{P(k)=A/k^3,\qquad \Delta^2(k)=k^3P(k)/(2\pi^2)=A/(2\pi^2).}
$$

Thus a [scale-invariant inflationary power spectrum](../../../../../../scale-invariant-inflationary-power-spectrum.md) has equal [variance](../../../../../../variance-split.md) per logarithmic [wavenumber](../../../../../../wavenumber.md) interval, rather than equal power per Fourier volume.

There is an important mathematical qualification to the literal [covariance](../../../../../../covariance.md) condition. A nonzero $k^{-3}$ [power spectrum](../../../../../../power-spectrum.md) over all scales has $C(0)=A\int dk/k/(2\pi^2)$, divergent at both endpoints; it is not the [covariance](../../../../../../covariance.md) of a finite-variance ordinary field. Moreover, exact dilation invariance of a continuous isotropic $C(r)$ makes it constant for $r>0$ and, by continuity, at zero: its spectrum can then consist only of a zero-mode delta measure. The nontrivial cosmological statement consequently concerns nonzero modes, with cutoffs or subtraction of an unobservable constant. For example the finite subtracted [covariance](../../../../../../covariance.md)

$$
C(r)-C(r_0)=\frac A{2\pi^2}\int_0^\infty\frac{dk}{k}\left[\frac{\sin kr}{kr}-\frac{\sin kr_0}{kr_0}\right]= -\frac A{2\pi^2}\log(r/r_0)
$$

is invariant under simultaneous rescaling of $r,r_0$. This is the precise [infrared qualification of a scale-invariant covariance](../../../../../../infrared-qualification-of-a-scale-invariant-covariance.md); a regulated unsubtracted $C(r)$ generally shifts by an additive constant under dilation. The formal derivation above gives the intended nonzero-mode scaling, with this qualification rather than an impossible finite-variance premise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
