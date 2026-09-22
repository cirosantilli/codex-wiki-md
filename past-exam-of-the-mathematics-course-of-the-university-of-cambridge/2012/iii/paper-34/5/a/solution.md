<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Before $\tau$, put $a_s=\sigma(Y_s)-\sigma(X_s)$ and $d_s=b_2(Y_s)-b_1(X_s)$, so $dZ_s=a_s\,dB_s+d_s\,ds$. For $Z_s\geq0$, the Lipschitz and drift-order hypotheses give $|a_s|\leq KZ_s$ and $d_s\geq b_1(Y_s)-b_1(X_s)\geq-LZ_s$. The derivatives of $f_\epsilon(z)=(z+\epsilon)^{-1}$ are $f'_\epsilon=-(z+\epsilon)^{-2}$ and $f''_\epsilon=2(z+\epsilon)^{-3}$. Itô's formula gives

$$
\boxed{f_\epsilon(Z_{t\wedge\tau})=f_\epsilon(z_0)-\int_0^{t\wedge\tau}\frac{a_s}{(Z_s+\epsilon)^2}\,dB_s+\int_0^{t\wedge\tau}\left(-\frac{d_s}{(Z_s+\epsilon)^2}+\frac{a_s^2}{(Z_s+\epsilon)^3}\right)ds.}
$$

The drift integrand is bounded above by

$$
\frac{LZ_s}{(Z_s+\epsilon)^2}+\frac{K^2Z_s^2}{(Z_s+\epsilon)^3}\leq\frac{L+K^2}{Z_s+\epsilon}.
$$

The stochastic integrand has magnitude at most $KZ_s/(Z_s+\epsilon)^2\leq K/(4\epsilon)$, so its integral on a finite horizon is a square-integrable [martingale](../../../../../../martingale-split.md) with mean zero. Global Lipschitz coefficients give finite second moments of the SDE solutions on finite horizons, which also justify the drift [expectation](../../../../../../expected-value.md); alternatively localize first and use boundedness of $f_\epsilon$ and Fatou. Since $Z_{t\wedge\tau}\geq0$, taking [expectations](../../../../../../expected-value.md) and replacing the stopped integral by the larger positive full-time bound yields the [reciprocal barrier proof of scalar diffusion comparison](../../../../../../reciprocal-barrier-proof-of-scalar-diffusion-comparison.md):

$$
\boxed{\mathbb E f_\epsilon(Z_{t\wedge\tau})\leq f_\epsilon(z_0)+(L+K^2)\int_0^t\mathbb E f_\epsilon(Z_{s\wedge\tau})\,ds.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
