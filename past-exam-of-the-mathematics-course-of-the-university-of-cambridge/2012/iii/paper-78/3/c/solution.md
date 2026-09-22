<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The zero-mean fluctuation is $W$, not the [refractive index](../../../../../../refractive-index.md) $n$: $\langle n\rangle=1$. Also the full [scattering potential](../../../../../../scattering-potential.md) has a nonzero mean and is not Gaussian:

$$
V=2\mu k_0^2W+\mu^2k_0^2W^2,\qquad \overline V=\mu^2k_0^2.
$$

The usual Gaussian closure requires $W$ to be a jointly [Gaussian random field](../../../../../../gaussian-random-field.md), not merely to have a [Gaussian distribution](../../../../../../normal-distribution.md) at each point. We first give the intended leading weak-fluctuation result with the linearized potential $V_1=2\mu k_0^2W$, then account for the quadratic term.

Keep the definitions $q,B$ from the preceding solution and let $\chi_1=B\int_D V_1(y)e^{-iq\cdot y}\,dy$. Because the incident field has unit modulus,

$$
I=\langle e^{\chi_1+\chi_1^*}\rangle,\qquad h(y)=B e^{-iq\cdot y}+B^*e^{iq\cdot y}=2\operatorname{Re}(B e^{-iq\cdot y}).
$$

The exponent is a real Gaussian linear functional $Z=\int_DhV_1$. If $C_W(y-z)=\langle W(y)W(z)\rangle$, the linearized potential has [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md) $C_1(s)=4\mu^2k_0^4 C_W(s)$. Complete the square in the one-dimensional Gaussian density of $Z$: $\langle e^Z\rangle=\exp(\langle Z\rangle+\operatorname{Var}Z/2)$. Here its mean is zero, so

$$
\boxed{I_{\mathrm{lin}}=\exp\left\{\frac12\int_D\int_D h(y)h(z)C_1(y-z)\,dy\,dz\right\}.}
$$

This is [Gaussian intensity in the first Rytov approximation](../../../../../../gaussian-intensity-in-the-first-rytov-approximation.md). In a more explicit complex notation, put

$$
J_1=\int_D\int_D C_1(y-z)e^{-iq\cdot(y-z)}\,dy\,dz,\qquad J_2=\int_D\int_D C_1(y-z)e^{-iq\cdot(y+z)}\,dy\,dz.
$$

Then

$$
\boxed{I_{\mathrm{lin}}=\exp\{|B|^2J_1+\operatorname{Re}(B^2J_2)\}.}
$$

The second term is the [pseudo-covariance of a complex random variable](../../../../../../pseudo-covariance.md) contribution. It does not vanish for an arbitrary finite real medium. The real-kernel expression shows that the combined exponent is nonnegative, even though its two complex-form contributions need not be separately nonnegative.

For the full potential, [Gaussian moment pairing theorem](../../../../../../isserlis-s-theorem.md) gives its centered [covariance function](../../../../../../covariance-function.md)

$$
C_V(s)=\operatorname{Cov}(V(y),V(y+s))=4\mu^2k_0^4C_W(s)+2\mu^4k_0^4C_W(s)^2.
$$

Its uncentered autocorrelation is $R_V(s)=C_V(s)+\mu^4k_0^4$. The first [Rytov approximation](../../../../../../rytov-approximation.md) is linear in $V$, but its intensity is an exponential average; applying a Gaussian formula exactly to this quadratic potential would be incorrect. A consistent expansion through order $\mu^2$ is

$$
\boxed{\log I=2\mu^2k_0^2\operatorname{Re}\left[B\int_De^{-iq\cdot y}\,dy\right]+\frac12\int_D\int_D h(y)h(z)C_1(y-z)\,dy\,dz+O(\mu^4).}
$$

The first term is the coherent mean-potential correction. Odd powers vanish by the symmetry of the joint Gaussian field. The variance term can equally use $C_V=R_V-\overline V^2$ through this order. Thus the mean shift must not be discarded while retaining the order-$\mu^2$ fluctuation intensity.

An exact expression within the far-field, first-[Rytov approximation](../../../../../../rytov-approximation.md) model is also available when the full $n^2$ is retained. Assume the restriction of $W$ to $D$ is a Gaussian element of the real [Hilbert space](../../../../../../hilbert-space-split.md) $L^2(D)$, with covariance operator $C$ of kernel $C_W(y-z)$. Let $H$ denote multiplication by $h$, $\ell_h=2\mu k_0^2h$, $Q=\mu^2k_0^2 C^{1/2}HC^{1/2}$ and $b_h=C^{1/2}\ell_h$. The [Gaussian quadratic exponential moment](../../../../../../gaussian-quadratic-exponential-moment.md) is

$$
\boxed{I=\det(I-2Q)^{-1/2}\exp\left[\frac12\langle b_h,(I-2Q)^{-1}b_h\rangle\right].}
$$

Here the determinant is the [Fredholm determinant](../../../../../../fredholm-determinant.md); require $I-2Q$ strictly positive for finiteness. Diagonalize the self-adjoint trace-class operator $Q$ and complete the square in each Gaussian coordinate to derive the formula. On a bounded $D$, unit pointwise variance makes $\operatorname{tr}C=|D|$, so the covariance is trace class under the stated measurable $L^2$ hypothesis. Small enough $\mu$ satisfies the positivity condition. Expanding the determinant and inverse recovers the preceding mean and covariance terms. For small $\mu$ this is also determined by the potential autocorrelation: since $C_W\in[-1,1]$,

$$
C_W(s)=\frac{-1+\sqrt{1+C_V(s)/(2k_0^4)}}{\mu^2},\qquad C_V=R_V-\mu^4k_0^4,
$$

using the branch near zero. This makes explicit the extra joint-Gaussian assumption behind an exact correlation-based answer.

Finally, Gaussian marginals alone are insufficient. Take $X\sim N(0,1)$ and independent random signs $S_j$. The stationary sequence $W_j=S_jX$ has Gaussian marginals and covariance $\langle W_iW_j\rangle=\delta_{ij}$, just like independent standard Gaussian variables. However $\langle e^{t(W_1+W_2)}\rangle=(1+e^{2t^2})/2$, whereas for the independent Gaussian pair it is $e^{t^2}$. The different intensities show why the joint hypothesis is needed. The mean-zero hint is interpreted for $W$, and the linearized Gaussian formula is not claimed to be exact for $V=k_0^2(n^2-1)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
