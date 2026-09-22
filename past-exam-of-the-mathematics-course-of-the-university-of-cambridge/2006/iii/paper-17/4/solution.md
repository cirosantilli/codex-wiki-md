<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On the standard [affine charts](../../../../../affine-chart-of-a-variety.md) $U_i=\{X_i\ne0\}$, use the formal frame $e_i=X_i^m$ and glue rank-one free [sheaves](../../../../../sheaf-mathematics.md) by

$$
e_j=(X_j/X_i)^m e_i.
$$

The transition functions are regular units on overlaps and satisfy the [cocycle](../../../../../cocycle.md) identity. This constructs the [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) $\mathcal O(m)$ as an [invertible sheaf](../../../../../line-bundle.md) for every integer $m$, including negative $m$.

On a nonempty $U$, a section has local expressions $h_i e_i$, where $h_i\in\mathcal O(U\cap U_i)$. Pulling to the punctured affine cone gives $h_i(X/X_i)X_i^m$. Their agreement on overlaps makes them one homogeneous rational function $r$ of degree $m$, regular on $\pi^{-1}U$. To make its [polynomial](../../../../../polynomial-split.md) representation explicit, write one nonzero local coefficient as $p(y)/q(y)$ in the affine coordinates. Homogenize $p,q$ to degrees $a,b$; the resulting rational expression is

$$
r=X_i^{m-a+b}\frac{p^{\mathrm{hom}}}{q^{\mathrm{hom}}}.
$$

If the exponent of $X_i$ is negative, move its power to the denominator. Cancel common factors; the greatest common divisor of [homogeneous polynomials](../../../../../homogeneous-polynomial.md) can be chosen homogeneous. Thus $r=F/G$ with $F,G$ coprime [homogeneous polynomials](../../../../../homogeneous-polynomial.md), $G\ne0$, and $\deg F-\deg G=m$.

Conversely, for such a homogeneous rational function regular on $\pi^{-1}U$, its coefficient $r/X_i^m$ is regular on $U\cap U_i$: restrict to the slice $X_i=1$. These coefficients obey the displayed transition rule and hence define a section. This proves the [homogeneous rational sections of a twisting sheaf](../../../../../homogeneous-rational-sections-of-a-twisting-sheaf.md) description in both directions, for arbitrary open $U$ rather than only a standard chart.

Now lift a regular degree-zero rational function $f=P/Q$ to the punctured cone. The quotient rule gives

$$
\frac{\partial f}{\partial X_i}=\frac{Q\,\partial_iP-P\,\partial_iQ}{Q^2}.
$$

This is a rational function homogeneous of degree $-1$. It is independent of the chosen representation because differentiation is a [derivation](../../../../../derivation-of-an-algebra.md) of the rational [function field](../../../../../function-field-of-an-algebraic-variety.md). It is regular wherever $f$ is regular: a derivation of a [polynomial](../../../../../polynomial-split.md) ring extends to each [localization](../../../../../localization-of-a-ring.md) by the quotient rule, and [regular functions](../../../../../regular-function.md) are locally such fractions. The preceding homogeneous-section description therefore proves

$$
\boxed{\partial_i f\in\Gamma(U,\mathcal O(-1))}.
$$

Zeros of a particular displayed denominator do not invalidate this argument; regularity is a property of the rational function, which can have another local representation.

The map $f\mapsto(\partial_0f,\ldots,\partial_nf)$ is a $k$-linear [sheaf](../../../../../sheaf-mathematics.md) derivation with values in $\mathcal O(-1)^{\oplus(n+1)}$. The [universal property of Kähler differentials](../../../../../universal-property-of-kahler-differentials.md) consequently defines

$$
D:\Omega^1_{\mathbb P^n}\longrightarrow\mathcal O(-1)^{\oplus(n+1)},\qquad
df\longmapsto(\partial_i f)_i.
$$

Multiplication by the coordinate section $X_i\in\Gamma(\mathbb P^n,\mathcal O(1))$ defines the other map

$$
\sigma:\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O,\qquad
(g_i)_i\longmapsto\sum_iX_i g_i.
$$

For a degree-$d$ homogeneous polynomial, differentiating each monomial gives $\sum_iX_i\partial_iP=dP$. Applying this to the equal-degree numerator and denominator gives $\sum_iX_i\partial_i f=0$ for degree-zero $f$, so $\sigma D=0$. This identity is valid in every characteristic.

To prove all the exactness assertions, fix $U_i$ and put $y_j=X_j/X_i$ for $j\ne i$. The [Kähler differential sheaf](../../../../../sheaf-of-kahler-differentials-over-a-field.md) is free there on $dy_j$, because a derivation of the polynomial ring is determined freely by its values on the coordinates. Trivialize each $\mathcal O(-1)$ with frame $X_i^{-1}$. In this frame,

$$
D(dy_j)=e_j-y_je_i,\qquad
\sigma((b_0,\ldots,b_n))=b_i+\sum_{j\ne i}y_jb_j,
$$

where $e_j$ now denotes the $j$th coordinate [vector](../../../../../vector.md) of the direct sum. The map $\sigma$ is surjective, since its $i$th coefficient is one. Its kernel consists exactly of tuples with $b_i=-\sum_{j\ne i}y_jb_j$, so the $n$ displayed [vectors](../../../../../vector.md) $e_j-y_je_i$ form a free [basis](../../../../../basis.md) of that kernel. The map $D$ sends the differential [basis](../../../../../basis.md) bijectively to this kernel [basis](../../../../../basis.md) and is therefore injective. Exactness on these charts proves the [cotangent Euler sequence in homogeneous coordinates](../../../../../cotangent-euler-sequence-in-homogeneous-coordinates.md)

$$
\boxed{0\to\Omega^1_{\mathbb P^n}\xrightarrow{D}
\mathcal O(-1)^{\oplus(n+1)}\xrightarrow{\sigma}\mathcal O\to0}.
$$

The proof uses no division by an integer and hence no characteristic-zero assumption.

For $n\ge1$, the [cohomology of twisting sheaves on projective space](../../../../../cohomology-of-twisting-sheaves-on-projective-space.md) gives

$$
h^q(\mathbb P^n,\mathcal O(m))=
\begin{cases}
\binom{m+n}{n},&q=0,\ m\ge0,\\
\binom{-m-1}{n},&q=n,\ m\le-n-1,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular, $H^0(\mathcal O)=k$, $H^{q>0}(\mathcal O)=0$, and $H^q(\mathcal O(-1))=0$ for every $q$. The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) of the displayed [Euler sequence](../../../../../euler-sequence.md) begins

$$
0\to H^0(\Omega^1)\to0\to k\to H^1(\Omega^1)\to0,
$$

and gives zero in the remaining degrees. Thus

$$
\boxed{\dim_k H^q(\mathbb P^n,\Omega^1_{\mathbb P^n})=
\begin{cases}1,&q=1,\\0,&q\ne1,\end{cases}\qquad(0\le q\le n,\ n\ge1)}.
$$

The nonzero group is generated by the connecting image of the section $1$ of $\mathcal O$. If $n=0$ is admitted, $\mathbb P^0$ is a point and its cotangent [sheaf](../../../../../sheaf-mathematics.md) is zero, so the sole requested group $H^0$ is zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
