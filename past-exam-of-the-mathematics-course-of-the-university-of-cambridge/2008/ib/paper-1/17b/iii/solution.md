<h1 id="17b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Incompressibility](../../../../../../incompressible-flow.md) makes each perturbation [velocity potential](../../../../../../velocity-potential.md) a [harmonic function](../../../../../../harmonic-function.md). A horizontal mode $e^{i(kx+\ell y)+st}$ has $q=\sqrt{k^2+\ell^2}>0$. Decay away from the interface selects $\varphi_1=A_1e^{qz}e^{i(kx+\ell y)+st}$ below and $\varphi_2=A_2e^{-qz}e^{i(kx+\ell y)+st}$ above. The [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) gives

$$
qA_1=(s+ikU_1)\zeta_0,\qquad-qA_2=(s+ikU_2)\zeta_0.
$$

Insert these into the [dynamic boundary condition for an inviscid interface](../../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md) and cancel a nonzero mode amplitude to obtain

$$
\rho_1(s+ikU_1)^2+\rho_2(s+ikU_2)^2+qg(\rho_1-\rho_2)=0.
$$

Writing $\rho_T=\rho_1+\rho_2$ and $\bar U=(\rho_1U_1+\rho_2U_2)/\rho_T$, completion of the square gives

$$
\rho_T(s+ik\bar U)^2-\frac{k^2\rho_1\rho_2}{\rho_T}(U_1-U_2)^2+qg(\rho_1-\rho_2)=0.
$$

Consequently

$$
\boxed{s=-ik\frac{\rho_1U_1+\rho_2U_2}{\rho_1+\rho_2}\ \pm\sqrt{\frac{k^2\rho_1\rho_2(U_1-U_2)^2}{(\rho_1+\rho_2)^2}-\frac{qg(\rho_1-\rho_2)}{\rho_1+\rho_2}}.}
$$

The imaginary advection term does not change growth rates. A mode grows exponentially precisely when the radicand is positive, equivalently

$$
\boxed{k^2\rho_1\rho_2(U_1-U_2)^2>qg(\rho_1^2-\rho_2^2).}
$$

If the upper fluid is heavier, every nonzero wavevector is unstable even without shear: this is [Rayleigh-Taylor instability](../../../../../../rayleigh-taylor-instability.md). If the lower fluid is heavier, gravity stabilizes sufficiently long waves, but any nonzero velocity difference destabilizes sufficiently short waves with $\ell=0$: this is [Kelvin-Helmholtz instability](../../../../../../kelvin-helmholtz-instability.md). For equal densities, shear destabilizes modes with $k\ne0$. A negative radicand gives purely imaginary frequencies and oscillatory modes; equality is the marginal threshold for exponential growth.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [17B](../../17b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
