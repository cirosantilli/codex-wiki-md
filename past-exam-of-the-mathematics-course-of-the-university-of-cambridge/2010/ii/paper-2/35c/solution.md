<h1 id="35c/solution">Solution</h1>

↑ **Parent:** [35C](../35c.md)

Each one-particle momentum state occupies volume $(2\pi\hbar)^3/V$ in momentum space. Counting the spherical shell gives the [density of states](../../../../../density-of-states.md)

$$
\boxed{g(\epsilon)=\frac{V}{2\pi^2\hbar^3}\frac{p(\epsilon)^2}{\epsilon'(p(\epsilon))}}.
$$

The increasing dispersion law permits inversion, and the density is zero below any minimum allowed energy. No additional spin degeneracy is included here.

For noninteracting particles, the classical Boltzmann sum factorizes into $z^N$. Dividing by $N!$ accounts for indistinguishability without quantum exchange corrections, giving the [partition function](../../../../../canonical-partition-function.md) $Z=z^N/N!$, with $z=\int g(\epsilon)e^{-\epsilon/(kT)}\,d\epsilon$. Differentiation with respect to inverse temperature gives

$$
\boxed{E=\frac Nz\int_0^\infty g(\epsilon)\epsilon e^{-\epsilon/(kT)}\,d\epsilon}.
$$

Fixed mode indices have momenta proportional to $L^{-1}$ because the boundary quantization condition fixes $pL/\hbar$. As $V=L^3$, $\partial p/\partial V=-p/(3V)$ and $\partial\epsilon/\partial V=-p\epsilon'(p)/(3V)$. The pressure $P=kT\,\partial_V\log Z$, evaluated by differentiating the mode sum, therefore obeys

$$
\boxed{PV=\frac N{3z}\int_0^\infty g(\epsilon)p\epsilon'(p)e^{-\epsilon/(kT)}\,d\epsilon}.
$$

For nonrelativistic particles $\epsilon=p^2/(2m)$, so $PV=2E/3$ and $E=3NkT/2$. For massless relativistic particles $\epsilon=cp$, so $PV=E/3$ and $E=3NkT$. **Both obey $PV=NkT$.**

The nonrelativistic [thermal wavelength](../../../../../thermal-de-broglie-wavelength.md) is **$\lambda_{\rm th}=h/\sqrt{2\pi mkT}$**, and $z=V/\lambda_{\rm th}^3$. If $\lambda_{\rm th}\ll(V/N)^{1/3}$, then $N\lambda_{\rm th}^3/V\ll1$: occupation per thermal quantum state is small. Wave packets scarcely overlap and exchange corrections to [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md) are negligible, justifying the classical formulas.

## ↑ Ancestors (10)

1. [35C](../35c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
