<h1 id="39a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [Fourier mode](../../../../../../fourier-mode.md) $u_m^n=\zeta^ne^{im\theta}$. Substitution gives

$$
\zeta^2-2[1-2\mu\sin^2(\theta/2)]\zeta+1=0.
$$

Its roots have product one. They lie on the [unit circle](../../../../../../complex-unit-circle.md) for all spatial frequencies precisely when $|1-2\mu\sin^2(\theta/2)|\leq1$, giving

$$
\boxed{0<\mu\leq1,\qquad\Delta t/\Delta x\leq1.}
$$

For $\mu>1$, the Nyquist frequency has a real reciprocal root pair with one root of modulus greater than one, giving exponential growth and instability.

The endpoint convention needs care in this two-step wave scheme: repeated unit roots occur at zero frequency, and also at the Nyquist frequency when $\mu=1$. They are not power-bounded for arbitrary two independent displacement sequences with a mesh-independent difference. With the usual initialization from displacement and velocity,

$$
u^1=u^0+k v^0+\frac\mu2\Delta_h^{\rm unscaled}u^0,
$$

each Fourier component satisfies $\widehat u^n=\cos(n\eta)\widehat u^0+k[\sin(n\eta)/\sin\eta]\widehat v^0$, where $\cos\eta=1-2\mu\sin^2(\theta/2)$. Taking the limiting values at repeated roots and using $|\sin(n\eta)|\leq n|\sin\eta|$ gives $|\widehat u^n|\leq|\widehat u^0|+nk|\widehat v^0|$. This is a uniform finite-time stability bound in the physical displacement/velocity data and includes $\mu=1$. A strict root-condition test for arbitrary two-level data must record the double-root qualification rather than calling that endpoint unconditionally power-bounded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
