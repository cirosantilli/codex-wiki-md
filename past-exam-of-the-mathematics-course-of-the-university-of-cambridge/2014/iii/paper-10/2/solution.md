<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**(A)** Use the [dimension of a bounded-total-degree polynomial space](../../../../../dimension-of-a-bounded-total-degree-polynomial-space.md). The monomials $x^iy^jz^k$ with $i+j+k\le d$ are a basis, and [stars and bars](../../../../../stars-and-bars-combinatorics.md) gives

$$
\dim\mathcal P_{\le d}(\mathbb R^3)=\binom{d+3}{3}.
$$

For a finite point set, the [polynomial evaluation map on a finite point set](../../../../../polynomial-evaluation-map-on-a-finite-point-set.md) is

$$
E_P:\mathcal P_{\le d}(\mathbb R^3)\longrightarrow\mathbb R^{P},
\qquad f\longmapsto(f(p))_{p\in P}.
$$

Its kernel is $V_d(P)$ and its rank is at most $|P|$, even when some conditions are dependent. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) therefore gives

$$
\dim V_d(P)\ge\binom{d+3}{3}-|P|.
$$

The original PDF specifies $V_4(P)$ here. With twelve points,

$$
\boxed{\dim V_4(P)\ge\binom73-12=23\ge5.}
$$

No general-position assumption is required.

**(B)** Let $L=|\mathcal L|\ge1$. We seek a [polynomial vanishing on a finite set of spatial lines](../../../../../polynomial-vanishing-on-a-finite-set-of-spatial-lines.md). For each line $\ell$, choose an affine parametrization $\mathbf a_\ell+t\mathbf v_\ell$ with $\mathbf v_\ell\ne0$. The [polynomial restriction to a line](../../../../../polynomial-restriction-to-a-line.md) of a degree-at-most-$d$ polynomial has form

$$
f(\mathbf a_\ell+t\mathbf v_\ell)=\sum_{j=0}^d c_{\ell,j}(f)t^j.
$$

Each coefficient is a linear functional of $f$. Setting all $d+1$ coefficients to zero is precisely the condition that $f$ vanish identically on $\ell$.

All lines together therefore impose at most $L(d+1)$ homogeneous linear conditions on the $\binom{d+3}{3}$-dimensional coefficient space. A nonzero solution exists whenever

$$
\binom{d+3}{3}>L(d+1),
\quad\text{equivalently}\quad
(d+2)(d+3)>6L.
$$

Take $d=\lceil\sqrt{6L}\rceil$. Then $d^2\ge6L$, so this strict inequality holds. Moreover

$$
d\le\sqrt{6L}+1\le(\sqrt6+1)\sqrt L<4\sqrt L.
$$

Thus the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) gives

$$
\boxed{\text{a nonzero }f\text{ with }\deg f<4|\mathcal L|^{1/2}
\text{ and }f|_\ell\equiv0\text{ for every }\ell\in\mathcal L.}
$$

Equivalently, one could impose vanishing at $d+1$ distinct points on each line and use the univariate root bound to force the entire restriction to vanish. For an empty line family, the constant polynomial one supplies vacuous vanishing; the strict degree comparison is understood for nonempty families.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
