<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use normalized [Haar measure](../../../../../../haar-measure.md) $m$ on the [real torus](../../../../../../real-torus.md). The integer [matrix](../../../../../../matrix.md) $A$ and its integer inverse induce a [toral automorphism](../../../../../../toral-automorphism.md); its determinant one preserves $m$. For $k\in\mathbb Z^n$, let $e_k(x)=e^{2\pi i k\cdot x}$. These [characters of a real torus](../../../../../../characters-of-a-real-torus.md) are an orthonormal basis, and

$$
e_k\circ T_A^j=e_{(A^T)^jk},\qquad
\int(e_k\circ T_A^j)\overline{e_\ell}\,dm
=\mathbf1_{\{(A^T)^jk=\ell\}}.
$$

Suppose no [eigenvalue](../../../../../../eigenvalue.md) of $A$ is a [root of unity](../../../../../../root-of-unity.md). For $k\ne0$, the frequency $(A^T)^jk$ can equal a fixed $\ell$ at most once. Otherwise two such times would give $(A^T)^qk=k$ for some $q>0$, forcing $A^q-I$ to be singular and an [eigenvalue](../../../../../../eigenvalue.md) of $A$ to have $q$th power one. Hence the displayed correlation eventually vanishes whenever a nonconstant character is involved. Constant characters give the product of their means.

Linearity gives mixing for finite [Fourier series](../../../../../../fourier-series-split.md). To pass to arbitrary $f,g\in L^2(m)$, approximate them by trigonometric polynomials. Composition with $T_A^j$ is an [isometry](../../../../../../isometry.md) of $L^2(m)$, so the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds the approximation errors uniformly in $j$. Let those errors tend to zero after taking the large-$j$ limit. Thus $\int(f\circ T_A^j)\overline g\,dm\to\int f\,dm\int\overline g\,dm$, which is the required [mixing measure-preserving transformation](../../../../../../strong-mixing.md) property.

Conversely, if an [eigenvalue](../../../../../../eigenvalue.md) is a [root of unity](../../../../../../root-of-unity.md), choose $q>0$ with $\det[(A^T)^q-I]=0$. This is an integer matrix, so its nullspace has a nonzero rational vector; clearing denominators gives $k\in\mathbb Z^n\setminus\{0\}$ with $(A^T)^qk=k$. The nonconstant character $e_k$ has mean zero, but

$$
\int(e_k\circ T_A^{jq})\overline{e_k}\,dm=1
$$

for every $j$. It cannot satisfy mixing. Therefore

$$
\boxed{T_A\text{ is mixing precisely when }\operatorname{spec}(A)\text{ contains no root of unity}.}
$$

[Hyperbolic toral automorphisms](../../../../../../hyperbolic-toral-automorphism.md) are mixing, but hyperbolicity is not necessary: this proof excludes periodic integer frequencies, not every eigenvalue of modulus one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
