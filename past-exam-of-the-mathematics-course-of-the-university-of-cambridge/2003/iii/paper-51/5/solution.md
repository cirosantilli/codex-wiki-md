<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use $[L_m,L_n]=(m-n)L_{m+n}+\frac c{12}(m^3-m)\delta_{m+n,0}$ and $L_n^\dagger=L_{-n}$. A normalized [highest-weight vector](../../../../../highest-weight-vector.md) obeys $L_0|h\rangle=h|h\rangle$ and $L_n|h\rangle=0$ for $n>0$. Its [Virasoro descendants](../../../../../virasoro-descendant.md) are products of negative modes. Their inner products are determined entirely by $c,h$ and the [Virasoro algebra](../../../../../virasoro-algebra.md); for example $\|L_{-1}|h\rangle\|^2=2h$, so unitarity requires $h\ge0$. An irreducible [unitary highest-weight Virasoro module](../../../../../unitary-highest-weight-virasoro-module.md) is the [Virasoro Verma module](../../../../../virasoro-verma-module.md) quotient by its null submodules, and its surviving [inner product](../../../../../inner-product.md) must be positive definite.

The classification for $c<1$ is the [Unitary Virasoro discrete series](../../../../../unitary-virasoro-discrete-series.md):

$$
\boxed{c=1-\frac6{m(m+1)},\qquad
h=h_{r,s}=\frac{[(m+1)r-ms]^2-1}{4m(m+1)}},
$$

where $m$ is an integer at least $2$, $1\le r\le m-1$, and $1\le s\le m$. The identification $(r,s)\sim(m-r,m+1-s)$ leaves $m(m-1)/2$ distinct modules. The two generating singular-vector levels are $rs$ and $(m-r)(m+1-s)$; all their [Virasoro descendants](../../../../../virasoro-descendant.md) are removed in the irreducible quotient. For $m=2$ the only module is the trivial $c=h=0$ module; for $m\ge3$ these are the nontrivial unitary discrete-series modules. There are no other irreducible unitary [highest-weight representations](../../../../../highest-weight-representation.md) with $c<1$. This is the classification theorem, rather than a condition inferred only from finitely many descendant norms.

At $c=1/2$, $m=3$ and the possible weights are

$$
\boxed{h=0,\qquad h=\frac12,\qquad h=\frac1{16}}.
$$

Construct them with a single free chiral [Majorana fermion](../../../../../majorana-spinor.md):

$$
\psi(z)=\sum_r b_rz^{-r-1/2},\qquad
\{b_r,b_s\}=\delta_{r+s,0},\qquad b_r^\dagger=b_{-r}.
$$

The [free chiral Majorana fermion conformal field theory](../../../../../free-chiral-majorana-fermion-conformal-field-theory.md) has $T=-:\psi\partial\psi:/2$. In the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md), $r\in\mathbb Z+1/2$, while in the [Ramond sector](../../../../../ramond-sector.md), $r\in\mathbb Z$. With positive modes moved to the right and the zero-mode product antisymmetrized, the corresponding generators are

$$
L_n=\frac12\sum_r\left(r-\frac n2\right):b_{n-r}b_r:+a\delta_{n,0},\qquad
a=0\text{ in NS},\quad a=\frac1{16}\text{ in R}.
$$

The oscillator relation gives $[L_n,b_r]=-(r+n/2)b_{n+r}$. The stress-tensor [operator product expansion](../../../../../operator-product-expansion.md), or the reordering of the quadratic generators, then gives the [Virasoro algebra](../../../../../virasoro-algebra.md) with $c=1/2$. One can check both constants directly in the ground states. In the [NS sector](../../../../../neveu-schwarz-sector.md),

$$
L_{-2}|0\rangle=\frac12b_{-3/2}b_{-1/2}|0\rangle,\qquad
\|L_{-2}|0\rangle\|^2=\frac14=\frac c2.
$$

In the [R sector](../../../../../ramond-sector.md), $b_0^2=1/2$ and $L_{-1}|R\rangle=\frac12 b_{-1}b_0|R\rangle$, whose norm squared is $1/8$. The relation $[L_1,L_{-1}]=2L_0$ requires $2h_R=1/8$, so $h_R=a=1/16$. Thus the [Ramond sector](../../../../../ramond-sector.md) zero-mode shift is essential.

The three constructions in [Ising Virasoro modules from a Majorana fermion](../../../../../ising-virasoro-modules-from-a-majorana-fermion.md) are explicit. The NS vacuum is a [highest-weight vector](../../../../../highest-weight-vector.md) of weight $0$. The state $b_{-1/2}|0\rangle$ is a [highest-weight vector](../../../../../highest-weight-vector.md) of weight $1/2$: applying any positive $L_n$ gives $-(n/2-1/2)b_{n-1/2}|0\rangle=0$, including the zero coefficient for $n=1$. Since $L_n$ is quadratic in fermions, the two cyclic modules lie in the even and odd [fermion parity](../../../../../fermion-parity.md) sectors, respectively. For R, choose a normalized ground state annihilated by all $b_n$ with $n>0$ and with $b_0|R\rangle=\pm|R\rangle/\sqrt2$. All positive $L_n$ annihilate it and its weight is $1/16$. The two zero-mode sign choices give isomorphic Virasoro modules; one choice suffices to construct the third module.

The oscillator inner products are positive, and each cyclic [highest-weight representation](../../../../../highest-weight-representation.md) just constructed is irreducible. Indeed any nonzero proper invariant graded submodule would have a lowest-energy vector $w$ of weight greater than the cyclic ground weight. Every positive $L_n$ annihilates $w$; thus $w$ is orthogonal to every negative-mode descendant of the original ground vector, by moving the modes across the [inner product](../../../../../inner-product.md). It is also orthogonal to that ground vector by its different $L_0$ eigenvalue. Since those [Virasoro descendants](../../../../../virasoro-descendant.md) span the cyclic module, $w$ would have zero norm, a contradiction. This proves irreducibility directly inside the positive [fermionic Fock space](../../../../../fermionic-fock-space.md).

In fact the cyclic modules fill the entire even NS, odd NS and chosen R [Fock spaces](../../../../../fock-space.md). Otherwise an orthogonal remaining lowest vector would be the ground vector of a further [unitary highest-weight Virasoro module](../../../../../unitary-highest-weight-virasoro-module.md); its weight would lie in $\mathbb Z_{>0}$, $1/2+\mathbb Z_{>0}$ or $1/16+\mathbb Z_{>0}$, respectively. None belongs to the classified list $\{0,1/2,1/16\}$. As a check, their [Virasoro characters](../../../../../virasoro-character.md), defined by $\chi_h(q)=\operatorname{Tr}q^{L_0-c/24}$, are

$$
\begin{aligned}
\chi_0(q)&=\frac{q^{-1/48}}2\left[\prod_{n\ge0}(1+q^{n+1/2})+\prod_{n\ge0}(1-q^{n+1/2})\right],\\
\chi_{1/2}(q)&=\frac{q^{-1/48}}2\left[\prod_{n\ge0}(1+q^{n+1/2})-\prod_{n\ge0}(1-q^{n+1/2})\right],\\
\chi_{1/16}(q)&=q^{1/24}\prod_{n\ge1}(1+q^n).
\end{aligned}
$$

The NS signs project onto even and odd occupation number; the R product uses the single chosen ground state. Null vectors of the abstract [Virasoro Verma modules](../../../../../virasoro-verma-module.md) are automatically zero in this construction. In particular $L_{-1}|0\rangle=0$, and the weight-$1/2$ and weight-$1/16$ ground states obey, respectively, $(L_{-2}-\frac34L_{-1}^2)|1/2\rangle=0$ and $(L_{-2}-\frac43L_{-1}^2)|1/16\rangle=0$, as is also verified by their level-two Gram matrices.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
