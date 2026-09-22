<h1 id="40e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Insert the Fourier mode

$$
u_m^n=\zeta^n e^{im\theta}
$$

into the [leapfrog advection scheme](../../../../../../leapfrog-advection-scheme.md). This gives

$$
\zeta^{n+1}
=\mu(e^{i\theta}-e^{-i\theta})\zeta^n+\zeta^{n-1},
$$

and hence the amplification polynomial

$$
\zeta^2-2i\mu\sin\theta\,\zeta-1=0.
$$

Its roots are

$$
\zeta_\pm=i\mu\sin\theta
\pm\sqrt{1-\mu^2\sin^2\theta}.
$$

If $0<\mu<1$, the square root is real for every $\theta$, and

$$
|\zeta_\pm|^2
=\mu^2\sin^2\theta+1-\mu^2\sin^2\theta=1.
$$

If $\mu>1$, choosing $|\sin\theta|>1/\mu$ makes the roots non-real multiples of $i$ with reciprocal moduli, one of which exceeds one, so the method is unstable.

The endpoint $\mu=1$ requires care. At $\theta=\pi/2$ the polynomial is

$$
(\zeta-i)^2,
$$

so a generic mode has the form $(c_1+c_2n)i^n$ and grows linearly. It satisfies the weaker test $|\zeta_\pm|\leq1$ often quoted in elementary Fourier analysis, but it violates the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) because the unit-modulus root is repeated. Therefore the rigorous uniform stability range for arbitrary two-level initial data is

$$
\boxed{0<\mu<1}.
$$

If “stable” is being used only for the non-amplification condition on root moduli, the conventionally quoted range is $0<\mu\leq1$, with $\mu=1$ a defective marginal endpoint rather than a uniformly stable case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40E](../../40e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
