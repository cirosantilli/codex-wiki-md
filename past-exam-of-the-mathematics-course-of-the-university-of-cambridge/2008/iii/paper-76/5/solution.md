<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a degree-$n$ [homogeneous polynomial](../../../../../homogeneous-polynomial.md), the [Euler homogeneous function theorem](../../../../../euler-theorem-for-homogeneous-functions.md) gives $\mathbf r\cdot\nabla H_n=nH_n$. On $r>0$ in three-dimensional [Euclidean space](../../../../../euclidean-norm.md),

$$
\nabla r^s=s r^{s-2}\mathbf r,\qquad \Delta r^s=s(s+1)r^{s-2}.
$$

Apply the [product rule for the Laplacian](../../../../../product-rule-for-the-laplacian.md):

$$
\Delta(r^sH_n)
=r^s\Delta H_n+2s r^{s-2}\mathbf r\cdot\nabla H_n+s(s+1)r^{s-2}H_n
=r^s\Delta H_n+s(2n+s+1)r^{s-2}H_n.
$$

For $s=-(2n+1)$ the second term vanishes. Hence [homogeneous harmonic inversion](../../../../../homogeneous-harmonic-inversion.md) gives

$$
\boxed{\Delta\!\left(\frac{H_n}{r^{2n+1}}\right)
=\frac{\Delta H_n}{r^{2n+1}},\qquad r>0.}
$$

The nonzero factor $r^{-(2n+1)}$ proves both directions: the transformed function is [harmonic](../../../../../harmonic-function.md) exactly when $\Delta H_n=0$ away from the origin. Since $\Delta H_n$ is a polynomial, vanishing on the punctured space makes it identically zero everywhere.

Equivalently, homogeneity shows that the [Kelvin transform](../../../../../kelvin-transform.md) is

$$
K_aH_n(\mathbf r)=\frac arH_n\!\left(\frac{a^2}{r^2}\mathbf r\right)
=a^{2n+1}\frac{H_n(\mathbf r)}{r^{2n+1}}.
$$

It sends a [regular solid harmonic](../../../../../regular-solid-harmonic.md) to an [irregular solid harmonic](../../../../../irregular-solid-harmonic.md), exchanging the radial powers $r^n$ and $r^{-n-1}$. The origin is excluded from the harmonicity statement: for example, the $n=0$ transform $1/r$ is harmonic only away from zero and has a distributional [Dirac delta function](../../../../../dirac-delta-function.md) source there.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
