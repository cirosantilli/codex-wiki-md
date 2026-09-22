<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Use [suffix notation](../../../../../einstein-notation.md), summing repeated indices from one to three. The contraction identity for the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) gives

$$
\begin{aligned}
(a\times b)\cdot(a\times c)
&=\epsilon_{ijk}\epsilon_{i\ell m}a_jb_ka_\ell c_m\\
&=(\delta_{j\ell}\delta_{km}-\delta_{jm}\delta_{k\ell})a_jb_ka_\ell c_m\\
&=(a\cdot a)(b\cdot c)-(a\cdot c)(b\cdot a)\\
&=b\cdot c-(a\cdot b)(a\cdot c).
\end{aligned}
$$

Here $a\cdot a=1$ because $a$ is a [unit vector](../../../../../unit-vector.md). For the second [cross product](../../../../../cross-product.md) identity, use $\epsilon_{ijk}\epsilon_{j\ell m}=\delta_{im}\delta_{k\ell}-\delta_{i\ell}\delta_{km}$:

$$
\begin{aligned}
[(a\times b)\times(a\times c)]_i
&=\epsilon_{ijk}\epsilon_{j\ell m}\epsilon_{knp}a_\ell b_ma_nc_p\\
&=b_i\epsilon_{\ell np}a_\ell a_nc_p-a_i\epsilon_{mnp}b_ma_nc_p\\
&=0-a_i\,b\cdot(a\times c)\\
&=[a\cdot(b\times c)]a_i.
\end{aligned}
$$

The first term vanishes because $a_\ell a_n$ is symmetric while the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is antisymmetric in those indices. The last equality uses cyclicity and antisymmetry of the [scalar triple product](../../../../../scalar-triple-product.md).

On the [unit sphere](../../../../../unit-sphere.md), a [great circle](../../../../../great-circle.md) has radius one, so the [spherical distance](../../../../../great-circle-distance.md) is its shorter arc length, equal to its central angle in $[0,\pi]$. The [dot product](../../../../../dot-product.md) of its endpoint [unit vectors](../../../../../unit-vector.md) is the cosine of that angle. Hence

$$
\boxed{\cos\delta(A,B)=a\cdot b.}
$$

For the angular formulas, take the ordinary nondegenerate convex minor [spherical triangle](../../../../../spherical-triangle.md): no pair of vertices is antipodal and the three vertices do not lie on one [great circle](../../../../../great-circle.md). These are needed for the displayed denominators and interior angles to be defined. Merely requiring three distinct points, as the PDF does, does not exclude degeneracy.

Put $p=\delta(A,B)$, $q=\delta(A,C)$ and $r=\delta(B,C)$. The outgoing unit tangent [vectors](../../../../../vector.md) at $A$ are

$$
u=\frac{b-(a\cdot b)a}{\sin p},\qquad v=\frac{c-(a\cdot c)a}{\sin q}.
$$

Their [dot product](../../../../../dot-product.md) is $\cos\alpha$. Equivalently, they are obtained from the normalized plane normals $a\times b$ and $a\times c$ by the same right-angle rotation in the tangent plane: $u=(a\times b)\times a/|a\times b|$, and similarly for $v$. Rotation preserves the [dot product](../../../../../dot-product.md), giving

$$
\cos\alpha=\frac{(a\times b)\cdot(a\times c)}{|a\times b|\,|a\times c|}.
$$

Since $|a\times b|=\sin p$ and $|a\times c|=\sin q$, the first proved identity becomes the [spherical law of cosines](../../../../../spherical-law-of-cosines.md):

$$
\boxed{\cos r=\cos p\cos q+\sin p\sin q\cos\alpha.}
$$

For the [spherical law of sines](../../../../../spherical-law-of-sines.md), take norms in the second proved identity. Writing $\tau=a\cdot(b\times c)$, and using $0<\alpha<\pi$, gives

$$
|\tau|=\sin p\sin q\sin\alpha.
$$

Cyclic permutation gives the corresponding formulas at $B$ and $C$. Dividing each by the positive product $\sin p\sin q\sin r$ proves

$$
\boxed{\frac{\sin\alpha}{\sin r}=\frac{\sin\beta}{\sin q}=\frac{\sin\gamma}{\sin p}=\frac{|\tau|}{\sin p\sin q\sin r}.}
$$

Finally, if all sides equal $s$, the [spherical law of cosines](../../../../../spherical-law-of-cosines.md) gives

$$
\cos\alpha=\frac{\cos s-\cos^2s}{\sin^2s}=\frac{\cos s}{1+\cos s}<\frac12,
$$

because $0<s<\pi$ makes $1+\cos s>0$ and $\cos s<1$. Cosine is strictly decreasing on $(0,\pi)$, so **every angle of a nondegenerate equilateral [spherical triangle](../../../../../spherical-triangle.md) is greater than $\pi/3$**.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
