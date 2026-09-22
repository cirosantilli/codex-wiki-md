<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose an ordered [affine open cover](../../../../../affine-open-cover.md) $\mathcal U=(U_i)$ of the [separated scheme](../../../../../separated-scheme.md). For a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) $\mathcal F$, the [Čech cochain groups](../../../../../cech-cochain-group.md) and differential are

$$
C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}\Gamma(U_{i_0}\cap\cdots\cap U_{i_p},\mathcal F),\qquad (dc)_{i_0\ldots i_{p+1}}=\sum_{j=0}^{p+1}(-1)^j c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

Terms corresponding to empty intersections are zero. Restriction commutes with restriction, so the terms in $d^2$ cancel in pairs. Define

$$
\boxed{H^p(X,\mathcal F)=\ker(d:C^p\to C^{p+1})/\operatorname{im}(d:C^{p-1}\to C^p).}
$$

Here an affine cover computes the Čech groups independently of the chosen affine cover. The reason is that finite intersections of affine opens in a [separated scheme](../../../../../separated-scheme.md) are affine: the intersection of two is the inverse image of the closed diagonal inside their affine product. Repeating gives the finite-intersection assertion. Quasi-coherent sheaves have no higher cohomology on these intersections. Apply an injective resolution of the [sheaf](../../../../../sheaf-mathematics.md) and form the double complex of its Čech cochains. In one direction the higher cohomology vanishes on every affine intersection, leaving precisely the displayed Čech complex. In the other direction the augmented Čech complex of the flasque resolution terms is exact, leaving the global-section resolution computing [sheaf cohomology](../../../../../sheaf-cohomology.md). Thus the two cohomologies agree, and refinement maps between affine-cover complexes induce the same groups. No such affine-intersection claim is being made for arbitrary nonseparated [schemes](../../../../../scheme.md).

For an [exact sequence](../../../../../exact-sequence.md) of quasi-coherent sheaves, sections on an affine intersection give an [exact sequence](../../../../../exact-sequence.md) of [modules](../../../../../module-mathematics.md), including surjectivity: this follows from the equivalence between quasi-coherent sheaves and [modules](../../../../../module-mathematics.md) on an [affine scheme](../../../../../affine-scheme.md). Taking products yields a [short exact sequence](../../../../../short-exact-sequence.md) of Čech cochain complexes. To describe the connecting map, lift a degree-$p$ cocycle in $C^p(\mathcal F'')$ to a cochain in $C^p(\mathcal F)$. Its differential maps to zero in $C^{p+1}(\mathcal F'')$ and therefore is a cocycle in $C^{p+1}(\mathcal F')$. Changing the lift adds a coboundary there; changing the original representative does the same. This defines the connecting homomorphism. The same lift-and-differentiate argument shows that a class is in its kernel exactly when it lifts to a cocycle in the middle complex, and verifies exactness at the other terms. Thus the resulting sequence is

$$
\boxed{\cdots\to H^p(X,\mathcal F')\to H^p(X,\mathcal F)\to H^p(X,\mathcal F'')\to H^{p+1}(X,\mathcal F')\to\cdots.}
$$

The sequence must be in quasi-coherent sheaves for this affine-sections argument; that is the intended category here.

For the punctured affine plane, use $U=D(x)$ and $V=D(y)$. Their [rings](../../../../../ring.md) are $k[x^{\pm1},y]$ and $k[x,y^{\pm1}]$, and the intersection [ring](../../../../../ring.md) is $k[x^{\pm1},y^{\pm1}]$. The two-open Čech complex is

$$
0\longrightarrow k[x^{\pm1},y]\oplus k[x,y^{\pm1}]\xrightarrow{(f,g)\mapsto g-f}k[x^{\pm1},y^{\pm1}]\longrightarrow0.
$$

Consequently

$$
H^1(X,\mathcal O_X)=\frac{k[x^{\pm1},y^{\pm1}]}{k[x^{\pm1},y]+k[x,y^{\pm1}]}.
$$

The denominator contains precisely the span of [Laurent monomials](../../../../../laurent-monomial.md) for which at least one exponent is nonnegative. Every [Laurent polynomial](../../../../../laurent-polynomial.md) has a unique monomial expansion, so the remaining monomials are linearly independent in the quotient and span it. Therefore

$$
\boxed{H^1(X,\mathcal O_X)=\bigoplus_{a,b\ge1}k[x^{-a}y^{-b}],}
$$

a countably infinite-dimensional [vector space](../../../../../vector-space-split.md). The brackets here denote cohomology classes. This calculates the [Čech cohomology of the punctured affine plane](../../../../../cech-cohomology-of-the-punctured-affine-plane.md), rather than merely observing that some nonzero cohomology exists.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
