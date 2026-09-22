<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Extend $q$ by zero to $x<0$. Its ordinary [Fourier transform](../../../../../../fourier-transform.md) is precisely the half-line transform $\widehat q$, so [Fourier inversion](../../../../../../fourier-inversion-theorem.md) gives the real-axis term for every interior point $x>0$. At $x=0$ the zero extension can have a jump; the interior inversion is the assertion needed here.

Write $k=u+iv$. The contour is the upper branch of a [hyperbola](../../../../../../hyperbola.md),

$$
v=\frac{\alpha+\sqrt{\alpha^2+4u^2}}2\geq\alpha,
$$

with $u$ increasing from $-\infty$ to $\infty$. In the region above it, $\nu(k)=i\alpha-k$ has nonpositive imaginary part. Therefore $\widehat q(\nu(k))$ is analytic there: its defining integral has factor $e^{iux-(v-\alpha)x}$ and converges for a sufficiently decaying $q$. Smoothness and integration by parts also give $\widehat q(\nu)=O(|\nu|^{-1})$ away from bounded spectral sets.

For an interior spatial point $x>0$, the factor $e^{ikx}$ decays exponentially as $\operatorname{Im}k\to+\infty$. Truncate the hyperbolic contour and close it above, using the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md); the closing segments vanish by this decay and the transform estimate. No poles occur in the enclosed region. Consequently the [half-line drift null contour identity](../../../../../../half-line-drift-null-contour-identity.md) is

$$
\boxed{\int_L e^{ikx}\widehat q(i\alpha-k)\,dk=0,\qquad x>0.}
$$

Adding any constant multiple of zero to [Fourier inversion](../../../../../../fourier-inversion-theorem.md) proves the proposed inversion, for every $c$. Oscillatory real-axis inversion may be understood by a Gaussian cutoff followed by its usual limit. The same contour argument allows a spectral multiplier analytic above $L$ with polynomial growth, because the exponential still controls the closing paths. We will need this slight extension for derivative boundary data.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
