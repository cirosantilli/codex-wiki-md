<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $v_i$ be the primitive lattice generator of the ray $\tau_i$. In the [toric divisor class sequence](../../../../../toric-divisor-class-sequence.md), the first map sends a [torus character](../../../../../characters-of-a-real-torus.md) exponent $m\in M$ to its [principal divisor on a toric variety](../../../../../principal-divisor-on-a-toric-variety.md):

$$
m\longmapsto\operatorname{div}(\chi^m)=\sum_i\langle m,v_i\rangle F_i.
$$

The second map sends an invariant [Weil divisor](../../../../../weil-divisor.md) to its class modulo principal divisors. Completeness makes the rays span $N_{\mathbb R}$, so the first map is injective. These are the maps in the given sequence; its exactness need not be reproved.

For $D=\sum_i r_iF_i$, let

$$
P_D=\{m\in M_{\mathbb R}:\langle m,v_i\rangle\ge-r_i\text{ for all }i\}.
$$

The [torus characters](../../../../../characters-of-a-real-torus.md) $\chi^m$ with $m\in P_D\cap M$ form a basis of $\mathcal L(D)=\{f\in\mathbb C(X):\operatorname{div}(f)+D\ge0\}\cup\{0\}$. This works for Weil divisors, not only for Cartier divisors. It is the character basis associated to the [lattice polytope of a toric divisor](../../../../../lattice-polytope-of-a-toric-divisor.md).

For a Cartier divisor, the [toric ampleness criterion](../../../../../toric-ampleness-criterion.md) is as follows. Each maximal cone $\sigma$ has local Cartier data $m_\sigma\in M$ satisfying $\langle m_\sigma,v_i\rangle=-r_i$ on its rays. The divisor is ample exactly when

$$
\langle m_\sigma,v_j\rangle>-r_j\qquad\text{for every ray }\tau_j\not\subseteq\sigma.
$$

Equivalently the support function is strictly concave, with these linear pieces. For a Q-Cartier Weil divisor use rational $m_\sigma$ and clear their denominators; the criterion means that a positive multiple is ample Cartier. An arbitrary Weil divisor need not be Q-Cartier, so this qualification cannot be omitted.

Take positive weights $q=(q_0,\ldots,q_n)$, reduced so their common greatest common divisor is one. A toric definition of [weighted projective space](../../../../../weighted-projective-space.md) uses

$$
\boxed{N=\mathbb Z^{n+1}/\mathbb Zq,\qquad v_i=\overline e_i,\qquad\Sigma=\{\operatorname{cone}(v_i:i\in I):I\subsetneq\{0,\ldots,n\}\}.}
$$

If the weights are well-formed, meaning $\gcd(q_0,\ldots,\widehat{q_i},\ldots,q_n)=1$ for every $i$, the $v_i$ are primitive: the quotient $N/\mathbb Zv_i$ has torsion of order that omitted-weight greatest common divisor. The lattice $N$ itself is free because $q$ is primitive. The positive relation $\sum_iq_iv_i=0$ implies that proper subsets generate pointed cones and that they meet along common faces. Completeness can be seen directly: represent a vector by real coordinates $a_i$ and subtract $\min_i(a_i/q_i)$ times $q$. The resulting coordinates are nonnegative and at least one is zero, placing the vector in one of the displayed cones. Their common-face property follows from this unique normalization of each class modulo $\mathbb Rq$. This gives the fan of the [well-formed weighted projective space](../../../../../well-formed-weighted-projective-space.md).

The dual lattice is

$$
M=\{m\in\mathbb Z^{n+1}:q\mathbin{\cdot}m=0\}.
$$

Its map in the divisor sequence is simply inclusion in $\mathbb Z^{n+1}$, so the homomorphism $a\mapsto q\mathbin{\cdot}a$ identifies the cokernel with $\mathbb Z$. It is onto by coprimality of all the weights. Thus

$$
\boxed{\operatorname{Cl}(X)\cong\mathbb Z,\qquad [F_i]=q_iH.}
$$

Choose integers $a_i$ by the Bezout identity $\sum_iq_ia_i=1$. Then $D=\sum_i a_iF_i$ explicitly represents the positive generator $H$.

To verify ampleness in the Weil/Q-Cartier sense, put $\ell=\operatorname{lcm}(q_0,\ldots,q_n)$. On the maximal cone omitting ray $j$, define

$$
m_j=\frac{\ell}{q_j}e_j-\ell a\in M.
$$

This is integral and has $q\mathbin{\cdot}m_j=\ell-\ell=0$. Its pairings with the included rays are $-\ell a_i$, while on the omitted ray they equal $-\ell a_j+\ell/q_j>-\ell a_j$. Consequently $\ell D$ is Cartier and ample by the numerical criterion. This is an explicit [class-group generator of a well-formed weighted projective space](../../../../../class-group-generator-of-a-well-formed-weighted-projective-space.md).

**The generator is generally ample Weil, not Cartier.** If the source's word “ample” is interpreted as requiring a Cartier divisor, its generator request is false in general: on $\mathbb P(1,1,2)$, take $D=F_0$. On the chart omitting the weight-two ray, the Cartier equations force $m=(-1,0,1/2)$, which is not in the integral dual lattice. Twice this datum is integral, so the class-one divisor has Cartier index two and no Cartier divisor generates its class group. With the usual ample-Q-Cartier-Weil interpretation, the construction above proves exactly the requested result. This distinction also explains the use of the divisorial spaces $\mathcal L(rD)$ rather than assuming an invertible sheaf $\mathcal O(D)$.

Finally let an ample divisor represent the class-group generator. Its class is the positive generator; the negative generator cannot be ample because a positive Cartier multiple has negative degree on the curves where the positive generator has positive degree. After replacing by a linearly equivalent invariant divisor, write it as $D=\sum a_iF_i$ with $\sum q_ia_i=1$. A character basis element of $\mathcal L(rD)$ has exponent $m\in M$ with $m_i+ra_i\ge0$. Set $b_i=m_i+ra_i$. Then $b\in\mathbb Z_{\ge0}^{n+1}$ and $\sum q_ib_i=r$. Conversely every nonnegative exponent vector of weighted degree $r$ gives the unique $m=b-ra\in M$. Therefore

$$
\chi^m\in\mathcal L(rD)\longmapsto X_0^{m_0+ra_0}\cdots X_n^{m_n+ra_n}
$$

is a bijection of bases in each degree. Adding $m$ and $r$ under multiplication adds these nonnegative exponent vectors, so it preserves products and the unit. A different linearly equivalent representative changes the basis by the corresponding rational-function power and gives the same graded-ring isomorphism. Hence **the divisorial section ring is the weighted polynomial ring**:

$$
\boxed{\bigoplus_{r\ge0}\mathcal L(rD)\cong k[X_0,\ldots,X_n],\qquad\deg X_i=q_i.}
$$

The character construction is defined over the ground field $k$, so this is an isomorphism of graded $k$-algebras. It proves the [divisorial section ring of a well-formed weighted projective space](../../../../../divisorial-section-ring-of-a-well-formed-weighted-projective-space.md) assertion even when its ample generator is not Cartier.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
