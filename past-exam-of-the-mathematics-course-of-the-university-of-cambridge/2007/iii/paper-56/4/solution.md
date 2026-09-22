<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $[Z_0:Z_1]$ be homogeneous coordinates on the [complex projective line](../../../../../complex-projective-line.md). The [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) $\mathcal O(-1)$ has fibre the line $\mathbb C(Z_0,Z_1)\subset\mathbb C^2$ over that point. Its dual is the [hyperplane line bundle](../../../../../hyperplane-line-bundle.md) $\mathcal O(1)$. Define the [tensor powers of the hyperplane line bundle](../../../../../tensor-powers-of-the-hyperplane-line-bundle.md) by $\mathcal O(n)=\mathcal O(1)^{\otimes n}$ for $n>0$, the trivial line bundle for $n=0$, and the appropriate power of $\mathcal O(-1)$ for $n<0$.

An explicit [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) construction uses the two charts $U_0=\{Z_0\ne0\}$ and $U_\infty=\{Z_1\ne0\}$ with coordinates $z=Z_1/Z_0$ and $w=Z_0/Z_1=1/z$. Choose [holomorphic local frames](../../../../../holomorphic-local-trivialization.md) related on the overlap by

$$
e_\infty=z^n e_0.
$$

This is consistent with the tautological frames $(1,z)$ and $(w,1)=z^{-1}(1,z)$ for $\mathcal O(-1)$. A [holomorphic section](../../../../../holomorphic-section.md) of $\mathcal O(n)$ is represented by entire chart functions satisfying

$$
f_0(z)e_0=f_\infty(1/z)e_\infty,\qquad f_\infty(w)=w^nf_0(1/w).
$$

Expand $f_0(z)=\sum_{k\geq0}a_kz^k$. Holomorphicity of $f_\infty$ at $w=0$ requires every power $w^{n-k}$ with $n-k<0$ to vanish. Thus for $n\geq0$, $f_0$ is exactly a polynomial of degree at most $n$. Conversely every such polynomial gives an entire $f_\infty$. Its coefficients supply the explicit isomorphism

$$
\boxed{H^0(\mathbb{CP}^1,\mathcal O(n))\simeq\mathbb C^{n+1}\qquad(n\geq0).}
$$

Equivalently, the global [holomorphic sections](../../../../../holomorphic-section.md) are the [homogeneous polynomials](../../../../../homogeneous-polynomial.md) $\sum_{k=0}^na_kZ_0^{n-k}Z_1^k$. For $n<0$, the same chart argument gives no nonzero global section.

For the first cohomology, use the [sheaf of holomorphic sections of a vector bundle](../../../../../sheaf-of-holomorphic-sections-of-a-vector-bundle.md) and its [Čech cohomology](../../../../../cech-cohomology.md) on this two-chart cover. A zero-cochain is a pair of entire chart functions $(h_0,h_\infty)$. A one-cochain is a function $g(z)$ holomorphic on $\mathbb C^*$, multiplied by $e_0$. There are no alternating two-cochains on a two-set cover, so every one-cochain is a cocycle. The coboundaries are

$$
(\delta h)(z)=z^nh_\infty(1/z)-h_0(z).
$$

Consequently the [holomorphic Laurent-series cohomology of twists on the projective line](../../../../../holomorphic-laurent-series-cohomology-of-twists-on-the-projective-line.md) is

$$
H^1(\mathbb{CP}^1,\mathcal O(n))
=\frac{\mathscr O(\mathbb C^*)}{\mathscr O(\mathbb C)+z^n\mathscr O(\mathbb C)(1/z)}.
$$

Here the last term means the set of functions $z^nh(1/z)$ with $h$ entire. The charts and their intersection are [Stein manifolds](../../../../../stein-manifold.md); [Cartan theorem B](../../../../../cartan-theorem-b.md) makes this cover acyclic for the line-bundle section sheaf, so this Čech group computes the sheaf cohomology.

Every $g$ on $\mathbb C^*$ has a [Laurent series](../../../../../laurent-series.md) $\sum_{k\in\mathbb Z}a_kz^k$ converging normally on compact annuli. Its nonnegative-power tail is an entire function of $z$ and can be removed by a finite-chart coboundary. Its tail with $k\leq n$ can be removed by $z^nh_\infty(1/z)$: the series $\sum_{k\leq n}a_kw^{n-k}$ is entire in $w$, because the inner Laurent radius is zero. Assign any overlapping removable powers to just one tail. The only possible remaining powers satisfy $n<k<0$.

If $n\geq-1$, there is no such integer, proving the requested vanishing:

$$
\boxed{H^1(\mathbb{CP}^1,\mathcal O(n))=0\qquad(n>-2).}
$$

For completeness, if $n\leq-2$, the remaining classes have basis $z^{n+1},\ldots,z^{-1}$ and dimension $-n-1$. None can be a coboundary, by uniqueness of Laurent coefficients. This also explains exactly why $-2$ is the threshold.

Finally, a global [holomorphic section](../../../../../holomorphic-section.md) of $\mathcal O(1)\oplus\mathcal O(1)$ is a pair of linear homogeneous polynomials:

$$
s([Z_0:Z_1])=(aZ_0+bZ_1,\ cZ_0+dZ_1).
$$

It vanishes at a projective point precisely when the nonzero vector $(Z_0,Z_1)^T$ belongs to the kernel of the coefficient matrix $M=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$. If $M$ has rank two there is no zero; if $M=0$ the section vanishes everywhere. Exactly one projective zero occurs precisely when the kernel is a one-dimensional line. Thus the [rank-one sections of two hyperplane line bundles](../../../../../rank-one-sections-of-two-hyperplane-line-bundles.md) are characterized by

$$
\boxed{ad-bc=0,\qquad(a,b,c,d)\ne(0,0,0,0).}
$$

Equivalently, $s=v\ell$, where $v\in\mathbb C^2$ is a fixed nonzero vector and $\ell$ is a nonzero section of $\mathcal O(1)$. Its single simple zero is the zero of $\ell$. This includes the case when one component is identically zero and the other is a nonzero linear form.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
