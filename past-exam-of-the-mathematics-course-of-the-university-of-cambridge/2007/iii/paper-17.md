# Paper 17

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper17.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper17.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $C=\check\sigma=\sigma^\vee$, $S=C\cap M$, and $U_\sigma=X_{\check\sigma}=\operatorname{Spec}k[S]$. The [semigroup algebra](../../../algebra.md#semigroup-algebra) has basis $\chi^m=x^m$, $m\in S$, with $\chi^m\chi^{m'}=\chi^{m+m'}$. The vertex assumption means that $\sigma$ is strongly convex, so its [dual cone](../../../toric-geometry.md#dual-cone) $C$ has full dimension. By the [Gordan lemma](../../../toric-geometry.md#gordan-lemma), $S$ is finitely generated: choose integral [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) generators and subtract integer parts of their nonnegative coefficients; the remainder lies in a bounded parallelepiped with only finitely many lattice points. This argument also applies when $C$ has [lineality space](../../../mathematical-optimization.md#lineality-space), by including generators in both directions there.

Choose an integral interior point $u\in C$. For every $m\in M$, both $tu$ and $tu+m$ belong to $S$ for all sufficiently large integers $t$. Thus $S-S=M$. Inverting all [monomial](../../../polynomial.md#monomial) generators of $k[S]$ gives the [group algebra](../../../associative-algebra.md#group-algebra) $k[M]$, which becomes $k[z_1^{\pm1},\ldots,z_n^{\pm1}]$ after a basis of $M$ is chosen. This proves the [dense torus of an affine toric variety](../../../toric-geometry.md#dense-torus-of-an-affine-toric-variety) assertion:

$$
\boxed{X_M=\operatorname{Spec}k[M]\cong(k^*)^n\text{ is a dense open subset of }U_\sigma.}
$$

Density follows because the [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) is of a domain. The algebra map $\chi^m\mapsto\chi^m\otimes\chi^m$ from $k[S]$ to $k[M]\otimes k[S]$ defines the extended [algebraic torus](../../../toric-geometry.md#algebraic-torus) action; on $X_M$ it is ordinary multiplication.

For a [face of a polyhedral cone](../../../toric-geometry.md#face-of-a-polyhedral-cone) $\nu\preceq C$, set $I_\nu=(\chi^m:m\in S\setminus\nu)$. The [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) property ensures that this is an ideal, and quotienting leaves $k[\nu\cap M]$. Hence $X_\nu=\operatorname{Spec}k[\nu\cap M]$ is a closed subvariety of $U_\sigma$. Its open [algebraic torus](../../../toric-geometry.md#algebraic-torus) consists of points where precisely the [monomials](../../../polynomial.md#monomial) with exponent in $\nu$ are nonzero.

To see that these [algebraic tori](../../../toric-geometry.md#algebraic-torus) exhaust the points, let $p$ be a point of $U_\sigma$ and put $S_p=\{m\in S:\chi^m(p)\ne0\}$. Multiplicativity gives $m+m'\in S_p$ if and only if both $m,m'\in S_p$. Thus $S_p$ is a [semigroup face](../../../algebra.md#face-of-an-additive-monoid). It is $S\cap\nu$ for a unique polyhedral [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) $\nu$: among a finite generating set of $S$, take the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) spanned by generators nonzero at $p$. A relation expressing a sum with a generator outside this [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) as a combination of generators inside would, after clearing rational denominators, contradict the displayed multiplicativity property. Therefore the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) is a [convex face](../../../mathematical-optimization.md#face-of-a-convex-set). Conversely, if $m\in S$ lies in that [convex face](../../../mathematical-optimization.md#face-of-a-convex-set), a positive multiple of $m$ is an integral sum of those generators, so $\chi^m(p)$ is nonzero as well. This also proves uniqueness.

The point $p$ lies in $X_M$ exactly when its [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) is all of $C$. Therefore

$$
\boxed{U_\sigma\setminus X_M=\bigcup_{\nu\prec C}X_\nu.}
$$

One can equivalently write this as the disjoint union of the open [algebraic tori](../../../toric-geometry.md#algebraic-torus) of the proper [convex faces](../../../mathematical-optimization.md#face-of-a-convex-set). For $\mu\in S$, the same description shows that $\chi^\mu(p)=0$ exactly when $\mu$ is not in the [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) supporting $p$. On every $X_\nu$ with $\mu\notin\nu$ the [monomial](../../../polynomial.md#monomial) vanishes identically. Consequently the [monomial zero locus in an affine toric variety](../../../toric-geometry.md#monomial-zero-locus-in-an-affine-toric-variety) is

$$
\boxed{V(\chi^\mu)_{\mathrm{red}}=\bigcup_{\substack{\nu\preceq C\\\mu\notin\nu}}X_\nu.}
$$

This is an equality of reduced subvarieties, or of their underlying closed sets. The principal subscheme itself may have multiplicity, as $x^2=0$ already shows on $\mathbb A^1$.

The [face duality for polyhedral cones](../../../toric-geometry.md#face-duality-for-polyhedral-cones) is the order-reversing pair of maps

$$
\boxed{\tau\preceq\sigma\ \longmapsto\ C\cap\tau^\perp,\qquad \nu\preceq C\ \longmapsto\ \sigma\cap\nu^\perp.}
$$

Their values are [convex faces](../../../mathematical-optimization.md#face-of-a-convex-set) because the relevant pairings are nonnegative and a sum pairs to zero only if each summand does. More explicitly, finitely many nonnegative exposing functionals can be summed to expose the indicated intersection. For a [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) $\tau$, choose $m_0\in C$ exposing it: $\tau=\sigma\cap m_0^\perp$. Then $m_0\in C\cap\tau^\perp$, so $\sigma\cap(C\cap\tau^\perp)^\perp\subseteq\tau$, while the reverse inclusion is immediate. Apply the same argument to a [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) $\nu$ of $C$, using $C^\vee=\sigma$, to prove the other composite is the identity. Inclusion reversal follows directly from annihilators. This proves the bijection, not just the existence of the maps.

For $\tau\preceq\sigma$, write $\nu=C\cap\tau^\perp$ and $L=M\cap\tau^\perp$. An exposing functional $m_0$ for $\tau$ is strictly positive on every [toric ray](../../../toric-geometry.md#ray-of-a-fan) outside $\tau$. Small perturbations of $m_0$ within $\tau^\perp$ preserve those finitely many strict inequalities, so $\nu$ has nonempty [relative interior](../../../mathematical-optimization.md#relative-interior) in $\tau^\perp$ and spans it. Therefore $\nu\cap M$ generates $L$, by the interior-point argument used above within that subspace. Thus the open [algebraic torus](../../../toric-geometry.md#algebraic-torus) of $X_\nu$ is $\operatorname{Spec}k[L]=X_{\tau^\perp}$. Here $X_{\tau^\perp}$ uses the lattice in the whole annihilator, rather than the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) semigroup. The sublattice $L$ is a [saturated sublattice](../../../group-theory.md#saturated-sublattice) of $M$ and consequently a direct summand; restriction $\operatorname{Hom}(M,k^*)\to\operatorname{Hom}(L,k^*)$ is surjective. The extended [algebraic torus](../../../toric-geometry.md#algebraic-torus) action is multiplication on this open [algebraic torus](../../../toric-geometry.md#algebraic-torus) and hence transitive. All other [monomials](../../../polynomial.md#monomial) vanish there. It follows that

$$
\boxed{O(\tau)=X_{\tau^\perp},\qquad F_\tau=\overline{O(\tau)}=X_{C\cap\tau^\perp}.}
$$

This is the [torus orbit-cone correspondence](../../../toric-geometry.md#orbit-cone-correspondence) and its [orbit closure in a toric variety](../../../toric-geometry.md#orbit-closure-in-a-toric-variety) description. Under [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) duality, $F_\gamma=\bigcup_{\eta\succeq\gamma}O(\eta)$.

Finally, choose integral $m_\tau\in C$ exposing $\tau$. Localizing $k[C\cap M]$ at $\chi^{m_\tau}$ gives $k[\tau^\vee\cap M]$: for $m\in\tau^\vee\cap M$, adding a sufficiently large multiple of $m_\tau$ makes it nonnegative on every [toric ray](../../../toric-geometry.md#ray-of-a-fan) of $\sigma$ outside $\tau$, while preserving nonnegativity on $\tau$. Hence $X_{\check\tau}=U_\tau=D(\chi^{m_\tau})$ is the usual affine open chart inside $U_\sigma$. An orbit $O(\gamma)$ belongs to it exactly when $\gamma\preceq\tau$. The requested [complement of an affine toric face chart](../../../toric-geometry.md#complement-of-an-affine-toric-face-chart) is therefore

$$
\boxed{X_{\check\sigma}\setminus X_{\check\tau}=\bigcup_{\substack{\gamma\preceq\sigma\\\gamma\npreceq\tau}}F_\gamma.}
$$

All sets on the right are closed, and if $\gamma$ is not contained in $\tau$, neither is any [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) containing $\gamma$. This justifies replacing the excluded orbits by their whole closures.

## 2

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

First suppose $\Delta$ has full dimension in $M_{\mathbb R}$. Form the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) over it in $M_{\mathbb R}\oplus\mathbb R$ and the graded [semigroup algebra](../../../algebra.md#semigroup-algebra)

$$
R_\Delta=\bigoplus_{l\ge0}\ \bigoplus_{m\in l\Delta\cap M} k\,\chi^m t^l,\qquad \deg(\chi^mt^l)=l,
$$

where degree zero contains only $k$. The lattice semigroup is finitely generated by the [Gordan lemma](../../../toric-geometry.md#gordan-lemma). The [projective toric variety of a lattice polytope](../../../toric-geometry.md#projective-toric-variety-of-a-lattice-polytope) is $\mathbb P_\Delta=\operatorname{Proj}R_\Delta$. Using all lattice points in all dilates avoids any assumption that the degree-one lattice points generate the ring.

For each vertex $v$ of $\Delta$, the degree-zero part after inverting $\chi^vt$ is

$$
(R_\Delta[(\chi^vt)^{-1}])_0=k[\operatorname{cone}(\Delta-v)\cap M].
$$

Indeed its exponents are $m-lv$ with $m\in l\Delta$. Conversely, every lattice point of the tangent [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) has this form for sufficiently large integral $l$. These charts cover the [Proj construction](../../../ringed-space.md#proj-construction): each point of a dilate is a rational convex combination of vertices, so some power of its [monomial](../../../polynomial.md#monomial) is a product of vertex [monomials](../../../polynomial.md#monomial). Their [dual cones](../../../toric-geometry.md#dual-cone) are the vertex [toric cones](../../../toric-geometry.md#cone-in-toric-geometry) of the inward [normal fan of a polytope](../../../toric-geometry.md#normal-fan-of-a-polytope). The normal [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) is complete because every [linear functional](../../../linear-algebra.md#linear-functional) on $\Delta$ attains its minimum on a [convex face](../../../mathematical-optimization.md#face-of-a-convex-set). This describes $\mathbb P_\Delta$ as a complete [toric variety](../../../toric-geometry.md#toric-variety). Translating $\Delta$ by $m_0\in M$ gives the graded isomorphism $(m,l)\mapsto(m+lm_0,l)$, so containing the origin is unnecessary. If $\Delta$ is not full-dimensional, translate a lattice vertex to zero and use $M\cap\operatorname{span}_{\mathbb R}(\Delta-\Delta)$; the construction is then complete of dimension $\dim\Delta$.

For the simplex in question put $Q=\prod_iq_i$. Its inequalities are $x_i\ge0$ and $\sum_iq_ix_i\le Q$, so its inward normal [toric rays](../../../toric-geometry.md#ray-of-a-fan) are $\mathbb R_+e_i$ and $\mathbb R_+(-q_1,\ldots,-q_n)$. Here the $e_i$ in the dual space denote the standard dual basis. Apply the real linear map $A(e_i)=e_i/q_i$. It carries these [toric rays](../../../toric-geometry.md#ray-of-a-fan) and their [convex face](../../../mathematical-optimization.md#face-of-a-convex-set) incidences to the standard [simplex fan](../../../toric-geometry.md#simplex-fan), with [toric rays](../../../toric-geometry.md#ray-of-a-fan) $e_1,\ldots,e_n,-\sum_i e_i$. The transported lattice is

$$
\boxed{N'=\bigoplus_{i=1}^n\frac1{q_i}\mathbb Z e_i\supseteq\mathbb Z^n,\qquad\mathbb P_\Delta\cong X_{\Sigma,N'}.}
$$

With $\gcd(q_1,\ldots,q_n)=1$, the primitive vectors of this [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) in $N'$ are $v_i=e_i/q_i$ and $v_0=-\sum_i e_i$. The latter is primitive because $\lambda\sum_i e_i\in N'$ requires each $\lambda q_i$ to be integral, whose smallest positive solution is $\lambda=1$. Their unique primitive relation is

$$
v_0+q_1v_1+\cdots+q_nv_n=0.
$$

Thus mutual coprimality beyond the displayed common gcd condition is not needed.

For a general complete [toric variety](../../../toric-geometry.md#toric-variety), introduce one variable $z_\rho$ for each [toric ray](../../../toric-geometry.md#ray-of-a-fan). Its [toric homogeneous coordinate ring](../../../toric-geometry.md#cox-ring), or [Cox ring](../../../toric-geometry.md#cox-ring), is

$$
\boxed{S=k[z_\rho:\rho\in\Sigma(1)],\qquad\deg z_\rho=[F_\rho]\in\operatorname{Cl}(X_\Sigma).}
$$

The [toric divisor class sequence](../../../toric-geometry.md#toric-divisor-class-sequence) is $0\to M\to\mathbb Z^{\Sigma(1)}\to\operatorname{Cl}(X_\Sigma)\to0$, where the first map is $m\mapsto(\langle m,v_\rho\rangle)_\rho$. Thus the graded piece $S_\alpha$ has basis the [monomials](../../../polynomial.md#monomial) $\prod z_\rho^{b_\rho}$ with $b_\rho\ge0$ and $\sum b_\rho[F_\rho]=\alpha$. For an invariant divisor $D=\sum a_\rho F_\rho$, [monomials](../../../polynomial.md#monomial) in degree $[D]$ correspond to [algebraic torus characters](../../../toric-geometry.md#algebraic-torus-character) $\chi^m$ through $b_\rho=a_\rho+\langle m,v_\rho\rangle\ge0$. This also identifies that graded piece with the global sections of $\mathcal O(D)$.

In our example $M'=(N')^*=\bigoplus_iq_i\mathbb Z e_i^*$, and its map to $\mathbb Z^{n+1}$ sends $\sum_iq_ib_ie_i^*$ to $(-\sum_iq_ib_i,b_1,\ldots,b_n)$. The quotient is therefore $\mathbb Z$, via $(c_0,\ldots,c_n)\mapsto c_0+\sum_iq_ic_i$. In particular $\deg z_0=1$ and $\deg z_i=q_i$, giving the explicit graded isomorphism

$$
\boxed{S\xrightarrow{\ \sim\ }k[Y_0,Y_1^{q_1},\ldots,Y_n^{q_n}],\qquad z_0\mapsto Y_0,\quad z_i\mapsto Y_i^{q_i}.}
$$

The target has the grading inherited from ordinary total degree in $k[Y_0,\ldots,Y_n]$. Its displayed generators are algebraically independent, which proves injectivity as well as surjectivity onto that subring.

To obtain the quotient, the [toric irrelevant ideal](../../../toric-geometry.md#toric-irrelevant-ideal) is generated by $\prod_{\rho\notin\sigma(1)}z_\rho$. Here each maximal [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) omits exactly one [toric ray](../../../toric-geometry.md#ray-of-a-fan), so it is $(z_0,\ldots,z_n)$, and the open set is $\mathbb A^{n+1}\setminus\{0\}$. The [diagonalizable algebraic group](../../../lie-theory.md#diagonalizable-group) with [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) group $\operatorname{Cl}(X)=\mathbb Z$ is $k^*$. Its action on the Cox coordinates is dictated by their degrees, namely

$$
\boxed{\lambda\cdot(y_0,\ldots,y_n)=(\lambda y_0,\lambda^{q_1}y_1,\ldots,\lambda^{q_n}y_n),\qquad\mathbb P_\Delta\cong\mathbb P(1,q_1,\ldots,q_n).}
$$

Here the $y_i$ name the independent Cox coordinates; the graded-subring realization above does not change their weights. More concretely, the quotient chart where $y_i\ne0$ has coordinate ring $(S[y_i^{-1}])_0$, the invariant ring for this action. These charts glue to $\operatorname{Proj}S$ and to the specified [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) charts. Positive weights make each orbit closed inside the punctured affine space, and in characteristic zero the finite stabilizers cause no failure of this [geometric quotient](../../../toric-geometry.md#geometric-quotient). This is the [weighted projective space](../../../toric-geometry.md#weighted-projective-space) construction.

## 3

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $u,v,w$ be the consecutive primitive [toric ray](../../../toric-geometry.md#ray-of-a-fan) vectors around the compact invariant curve $F=F_v$. Smoothness gives oriented determinants $\det(u,v)=\det(v,w)=1$, hence $u+w=bv$ for an integer $b$. Choose an [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) $m$ with $\langle m,u\rangle=0$ and $\langle m,v\rangle=1$. The [principal divisor on a toric variety](../../../toric-geometry.md#principal-divisor-on-a-toric-variety) has coefficient one at $F$, coefficient $b$ at $F_w$, and zero at $F_u$. The other invariant curves do not meet $F$, while each adjacent one meets it transversely once. Intersecting this [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) with the proper curve $F$ gives $0=F^2+b$. This proves the [self-intersection formula for a toric surface divisor](../../../toric-geometry.md#self-intersection-formula-for-a-toric-surface-divisor) even when the ambient surface is not complete.

If $F^2=-1$, then $b=1$ and $v=u+w$. The vectors $u,w$ form a lattice basis since $\det(u,w)=1$, and their [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) is the union of the two [toric cones](../../../toric-geometry.md#cone-in-toric-geometry) adjacent to $v$. Deleting $v$ is consequently a smooth [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) coarsening. Its inverse is precisely the [toric blowup at a torus-fixed point](../../../toric-geometry.md#toric-blowup-at-a-torus-fixed-point), obtained by inserting the sum of the two primitive basis vectors. Conversely, that insertion gives $u+w=v$, and hence [algebraic self-intersection](../../../algebraic-geometry.md#self-intersection-of-an-algebraic-curve) $-1$. Thus the [toric contraction of a minus-one curve](../../../toric-geometry.md#toric-contraction-of-a-minus-one-curve) satisfies

$$
\boxed{F\text{ contracts torically to a smooth point}\ \Longleftrightarrow\ F^2=-1.}
$$

For the cyclic quotient description, first take a strongly convex [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) of dimension two. Write its primitive boundary vectors as $a,b$ and put $N_0=\mathbb Za+\mathbb Zb$, $r=[N:N_0]$. Since $a$ is primitive, extend it to a basis of $N$ and write $b=ua+rc$ with $\gcd(u,r)=1$. Thus $N/N_0$ is cyclic of order $r$. In the lattice $N_0$, the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) is smooth and its [toric variety](../../../toric-geometry.md#toric-variety) is $\mathbb A^2$. Passing to the larger lattice $N$ takes the finite quotient whose invariant [monomials](../../../polynomial.md#monomial) are precisely those in the smaller dual lattice $M=N^*\subset N_0^*$. Relative to the two boundary coordinates, $c=(b-ua)/r$, so a generator acts with weights $(-u,1)$ modulo $r$. Replacing that generator by a suitable power makes the first weight one and the second some $q$ with $0<q<r$ and $\gcd(q,r)=1$. Therefore, for the singular case,

$$
\boxed{U_\sigma\cong\mathbb A^2/\mu_r,\qquad\zeta\cdot(x,y)=(\zeta x,\zeta^q y).}
$$

The [cyclic quotient surface singularity](../../../toric-geometry.md#cyclic-quotient-surface-singularity) can equivalently be described by the first-quadrant [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) in

$$
L=\mathbb Z^2+\mathbb Z\frac{(1,q)}r,\qquad L^*=\{(i,j)\in\mathbb Z^2:i+qj\equiv0\pmod r\}.
$$

Indeed its coordinate ring is $k[x^iy^j:i,j\ge0,\ i+qj\equiv0\pmod r]=k[x,y]^{\mu_r}$. Characteristic zero ensures the stated ordinary finite-group quotient interpretation.

The restriction to singular [toric cones](../../../toric-geometry.md#cone-in-toric-geometry) of dimension two is necessary for $r>1$. A smooth [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) has $r=1$ and gives $\mathbb A^2$ with the trivial quotient. A [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) of dimension one gives $\mathbb A^1\times k^*$, and the zero [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) gives $(k^*)^2$. These latter surfaces cannot be a quotient of the displayed kind, since they have nonconstant invertible [regular functions](../../../ringed-space.md#regular-function), whereas $k[x,y]^{\mu_r}$ has only constant units. Thus the blanket affine-surface wording requires these separate cases.

For the singular case, compute the [negative continued fraction](../../../number-theory.md#negative-continued-fraction) by the ceiling form of the [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm). Start with $a_0=r$, $a_1=q$, and, while $a_i>0$, set

$$
b_i=\left\lceil\frac{a_{i-1}}{a_i}\right\rceil,\qquad a_{i+1}=b_ia_i-a_{i-1}.
$$

Then $0\le a_{i+1}<a_i$, so the process terminates at $a_{s+1}=0$. The gcd is unchanged at each step, hence $a_s=1$. Since $a_{i-1}>a_i>0$, every $b_i\ge2$. Rearranging the recurrence gives

$$
\boxed{\frac rq=[b_1,\ldots,b_s]^-=b_1-\frac1{b_2-\dfrac1{\cdots-1/b_s}}.}
$$

Now define lattice vectors

$$
v_0=(0,1),\qquad v_1=\frac{(1,q)}r,\qquad v_{i+1}=b_iv_i-v_{i-1}.
$$

To verify this [Hirzebruch–Jung resolution](../../../toric-geometry.md#hirzebruch-jung-resolution) algorithm, write $v_i=(p_i,a_i)/r$ with $p_0=0$, $p_1=1$ and $p_{i+1}=b_ip_i-p_{i-1}$. Induction gives $a_i\equiv qp_i\pmod r$, so $v_i\in L$. It also gives $p_i a_{i+1}-a_i p_{i+1}=-r$. Thus every adjacent pair has absolute determinant $1/r$, the covolume of $L$, and is a basis of $L$. The $p_i$ increase strictly, while the $a_i$ decrease to zero, so these [toric rays](../../../toric-geometry.md#ray-of-a-fan) occur in order inside the first quadrant. At termination, $a_s=1$ and the determinant identity gives $p_{s+1}=r$, hence $v_{s+1}=(1,0)$. All boundary and inserted vectors are primitive because they occur in lattice bases.

Subdivide the quadrant by $v_1,\ldots,v_s$. Every resulting [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) is smooth by the [smoothness criterion for a toric variety](../../../toric-geometry.md#smoothness-criterion-for-a-toric-variety), and the [fan subdivision](../../../toric-geometry.md#fan-subdivision) gives a proper birational [toric morphism](../../../toric-geometry.md#toric-morphism), hence a resolution. Each interior [toric ray](../../../toric-geometry.md#ray-of-a-fan) has a complete one-dimensional star, so its [exceptional curve of a surface resolution](../../../algebraic-geometry.md#exceptional-curve-of-a-surface-resolution) is $\mathbb P^1$. The recurrence yields

$$
\boxed{F_i^2=-b_i\le-2,\qquad F_i\cdot F_{i+1}=1,\qquad F_i\cdot F_j=0\ (|i-j|>1).}
$$

This proves minimality: no [exceptional curve of a surface resolution](../../../algebraic-geometry.md#exceptional-curve-of-a-surface-resolution) can be contracted to a smooth point by the [Castelnuovo contraction criterion](../../../algebraic-geometry.md#castelnuovo-contraction-criterion). There is also a direct [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) check. For fixed $i$, the determinants of $v_i$ with $v_{i+h}$, measured in units of the lattice covolume, satisfy the same recurrence with coefficients at least two and initial values zero and one. They are at least $h$. Omitting any intervening [toric ray](../../../toric-geometry.md#ray-of-a-fan) therefore leaves a [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) of determinant at least two, so no nontrivial coarsening is smooth. Thus this is the [minimal resolution of a cyclic quotient surface singularity](../../../toric-geometry.md#hirzebruch-jung-resolution).

If all exceptional [algebraic self-intersections](../../../algebraic-geometry.md#self-intersection-of-an-algebraic-curve) are $-2$, all $b_i=2$ and induction gives $[2,\ldots,2]^-= (s+1)/s$. Since $r,q$ are coprime, this forces $r=s+1$, $q=s$. Conversely $r/(r-1)$ has exactly $r-1$ coefficients equal to two. Therefore

$$
\boxed{F_i^2=-2\text{ for every exceptional curve}\ \Longleftrightarrow\ q=r-1.}
$$

For the final [toric fan](../../../toric-geometry.md#fan-in-toric-geometry), the minimal smooth [fan subdivision](../../../toric-geometry.md#fan-subdivision) of the [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) from $(0,1)$ to $(r,1)$ inserts the [toric rays](../../../toric-geometry.md#ray-of-a-fan) $(j,1)$ for $1\le j<r$. Adjacent determinants have absolute value one, and $(j-1,1)+(j+1,1)=2(j,1)$, so its inserted curves have [algebraic self-intersection](../../../algebraic-geometry.md#self-intersection-of-an-algebraic-curve) $-2$ and it is the minimal [fan subdivision](../../../toric-geometry.md#fan-subdivision) just described. The second original [toric cone](../../../toric-geometry.md#cone-in-toric-geometry), from $(r,1)$ to $(1,0)$, is already smooth.

Write $v_j=(j,1)$ and $e=(1,0)$. In the resolved [toric fan](../../../toric-geometry.md#fan-in-toric-geometry), the rightmost interior [toric ray](../../../toric-geometry.md#ray-of-a-fan) obeys $v_{r-1}+e=v_r$, so its curve has [algebraic self-intersection](../../../algebraic-geometry.md#self-intersection-of-an-algebraic-curve) $-1$ and can be blown down to a smooth point. After deleting it, the same relation $v_{r-2}+e=v_{r-1}$ applies to the new rightmost interior [toric ray](../../../toric-geometry.md#ray-of-a-fan). Continue deleting $v_r,v_{r-1},\ldots,v_1$ in that order. Each deletion is the inverse of a [toric blowup at a torus-fixed point](../../../toric-geometry.md#toric-blowup-at-a-torus-fixed-point). The last [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) has only the quadrant [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) and defines $\mathbb A^2$. Consequently

$$
\boxed{X_{\Sigma'}\longrightarrow\mathbb A^2\text{ is the composite of exactly }r\text{ smooth-point toric blowdowns}.}
$$

All maps induce the identity on the dense [algebraic torus](../../../toric-geometry.md#algebraic-torus), so this composite is the same morphism as $X_{\Sigma'}\to X_\Sigma\to\mathbb A^2$. The intermediate smooth [toric fans](../../../toric-geometry.md#fan-in-toric-geometry) need not include the singular [toric fan](../../../toric-geometry.md#fan-in-toric-geometry) $\Sigma$.

## 4

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The dense [algebraic torus](../../../toric-geometry.md#algebraic-torus) has coordinate ring $k[M]$, a [Laurent polynomial ring](../../../commutative-algebra.md#laurent-polynomial-ring) and hence a [unique factorization domain](../../../algebra.md#unique-factorization-domain). Its [divisor class group](../../../algebraic-geometry.md#divisor-class-group) is therefore zero. Restrict an arbitrary [Weil divisor](../../../algebraic-geometry.md#weil-divisor) $D$ to the [algebraic torus](../../../toric-geometry.md#algebraic-torus) and choose a [rational function on an algebraic variety](../../../algebraic-geometry.md#rational-function-on-an-algebraic-variety) $f$ whose divisor there is $D|_T$. Then $D-\operatorname{div}(f)$ is supported on the [algebraic torus](../../../toric-geometry.md#algebraic-torus) boundary. The prime divisors in that boundary are precisely the $F_j$ corresponding to the [toric rays](../../../toric-geometry.md#ray-of-a-fan), by the [torus orbit-cone correspondence](../../../toric-geometry.md#orbit-cone-correspondence). Consequently

$$
\boxed{D\sim\sum_{j=1}^d a_jF_j\quad\text{for some }a_j\in\mathbb Z.}
$$

Since the variety is smooth, every [Weil divisor](../../../algebraic-geometry.md#weil-divisor) is Cartier. This gives invariant representatives for all divisor classes, without assuming that the original divisor was invariant.

Now use such a representative. The associated vector space is

$$
L(D)=\{f\in k(X)^*: \operatorname{div}(f)+D\ge0\}\cup\{0\}=H^0(X,\mathcal O_X(D)).
$$

The [principal divisor on a toric variety](../../../toric-geometry.md#principal-divisor-on-a-toric-variety) formula gives $\operatorname{div}(\chi^m)=\sum_j\langle m,e_j\rangle F_j$. Define the [lattice polytope of a toric divisor](../../../toric-geometry.md#lattice-polytope-of-a-toric-divisor)

$$
P_D=\{m\in M_{\mathbb R}:\langle m,e_j\rangle\ge-a_j\text{ for every }j\}.
$$

For a maximal [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) $\sigma$, its basic [toric ray](../../../toric-geometry.md#ray-of-a-fan) vectors are a basis of $N$, so there is a unique integral $m_\sigma$ with $\langle m_\sigma,e_j\rangle=-a_j$ on its [toric rays](../../../toric-geometry.md#ray-of-a-fan). The [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) $\chi^{m_\sigma}$ is a local frame for $\mathcal O(D)$ on $U_\sigma$. Every global section restricts on the [algebraic torus](../../../toric-geometry.md#algebraic-torus) to a finite [Laurent polynomial](../../../polynomial.md#laurent-polynomial) $\sum_m c_m\chi^m$. Relative to this frame, regularity on $U_\sigma$ means $\sum_m c_m\chi^{m-m_\sigma}\in k[\sigma^\vee\cap M]$. Since distinct [algebraic torus characters](../../../toric-geometry.md#algebraic-torus-character) are independent, this holds exactly when each exponent with nonzero coefficient satisfies the inequalities for the [toric rays](../../../toric-geometry.md#ray-of-a-fan) of $\sigma$. Taking all charts proves

$$
\boxed{L(D)=\bigoplus_{m\in P_D\cap M}k\chi^m.}
$$

Completeness makes $P_D$ bounded when nonempty: a nonzero recession vector would be nonnegative on every [toric ray](../../../toric-geometry.md#ray-of-a-fan) of a complete [toric fan](../../../toric-geometry.md#fan-in-toric-geometry), and therefore on all of $N_{\mathbb R}$, which is impossible. The displayed space is consequently finite-dimensional.

At the torus-fixed point $p_\sigma$ in the smooth chart $U_\sigma\cong\mathbb A^n$, a section $\chi^m$ has local [monomial](../../../polynomial.md#monomial) $\chi^{m-m_\sigma}$. Its value is nonzero exactly when this [monomial](../../../polynomial.md#monomial) is constant, namely when $m=m_\sigma$. Thus if the [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor) has no base point, some section is nonzero at $p_\sigma$, forcing $m_\sigma\in P_D$. Conversely, if $m_\sigma\in P_D$ for every maximal [toric cone](../../../toric-geometry.md#cone-in-toric-geometry), its [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) is a global section whose local expression on $U_\sigma$ is one. It therefore vanishes nowhere on that whole chart, and these charts cover $X$. This proves the [toric basepoint-free criterion](../../../cartier-divisor.md#toric-basepoint-free-criterion):

$$
\boxed{|D|\text{ is basepoint-free}\ \Longleftrightarrow\ \forall\sigma\in\Sigma(n),\ \langle m_\sigma,e_j\rangle\ge-a_j\text{ for all }j,\text{ with equality on }\sigma.}
$$

The analogous [toric ampleness criterion](../../../cartier-divisor.md#toric-ampleness-criterion), stated without proof, replaces the inequalities off $\sigma$ by strict ones:

$$
\boxed{D\text{ is ample}\ \Longleftrightarrow\ \forall\sigma\in\Sigma(n),\ \langle m_\sigma,e_j\rangle=-a_j\text{ on }\sigma,\quad\langle m_\sigma,e_j\rangle>-a_j\text{ off }\sigma.}
$$

Equivalently, the [normal fan of a polytope](../../../toric-geometry.md#normal-fan-of-a-polytope) $P_D$ is exactly $\Sigma$.

For the final [fan subdivision](../../../toric-geometry.md#fan-subdivision), take $n\ge2$ so that $\tilde e$ is a new [toric ray](../../../toric-geometry.md#ray-of-a-fan), as the construction requires. The vectors $e_1,\ldots,e_n$ are a lattice basis, so their sum is primitive. Replacing any one basis vector by this sum gives another basis. Thus the [star subdivision](../../../toric-geometry.md#star-subdivision) gives a smooth [toric blowup at a torus-fixed point](../../../toric-geometry.md#toric-blowup-at-a-torus-fixed-point) $\pi:X_{\Sigma'}\to X_\Sigma$, with [algebraic exceptional divisor](../../../algebraic-geometry.md#algebraic-exceptional-divisor) $E=\tilde F$. On the old chart, a local equation of $D$ is $\chi^{-m_\sigma}$, whose order on the new [toric ray](../../../toric-geometry.md#ray-of-a-fan) is $-\langle m_\sigma,\tilde e\rangle=\sum_{i=1}^n a_i=a$. All old [toric ray](../../../toric-geometry.md#ray-of-a-fan) coefficients are unchanged. Therefore

$$
\boxed{D'=\pi^*D.}
$$

We prove ampleness of $D_c=cD'-E$ directly by inequalities, giving the [ample divisor after blowing up a torus-fixed point](../../../toric-geometry.md#ample-divisor-after-blowing-up-a-torus-fixed-point) result.

Let $u_1,\ldots,u_n$ be the basis of $M$ dual to $e_1,\ldots,e_n$. On the new maximal [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) $\sigma_i$, which omits $e_i$, the required local [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) is

$$
m_{i,c}=cm_\sigma+u_i.
$$

Indeed its pairings on $e_j$, $j\ne i$, are $-ca_j$, while its pairing on $\tilde e$ is $-ca+1$, exactly the negative of the new coefficient $ca-1$. Its inequality on the omitted old [toric ray](../../../toric-geometry.md#ray-of-a-fan) has strict gap one:

$$
\langle m_{i,c},e_i\rangle+ca_i=1.
$$

For any [toric ray](../../../toric-geometry.md#ray-of-a-fan) $e_j$ outside the original [toric cone](../../../toric-geometry.md#cone-in-toric-geometry), put $\delta_j=\langle m_\sigma,e_j\rangle+a_j$. The original ampleness gives positive integers $\delta_j$, and the new strict gaps are

$$
\langle m_{i,c},e_j\rangle+ca_j=c\delta_j+\langle u_i,e_j\rangle>0
$$

for all sufficiently large $c$.

For any unchanged maximal [toric cone](../../../toric-geometry.md#cone-in-toric-geometry) $\eta\ne\sigma$, the local [algebraic torus character](../../../toric-geometry.md#algebraic-torus-character) is $cm_\eta$. All strict inequalities on old [toric rays](../../../toric-geometry.md#ray-of-a-fan) follow from those for $D$. Its inequality on the new [toric ray](../../../toric-geometry.md#ray-of-a-fan) has gap

$$
\langle cm_\eta,\tilde e\rangle+ca-1=c\epsilon_\eta-1,\qquad\epsilon_\eta=\sum_{i=1}^n(\langle m_\eta,e_i\rangle+a_i).
$$

Each summand is nonnegative, and at least one is positive because $\eta\ne\sigma$ cannot contain all its [toric rays](../../../toric-geometry.md#ray-of-a-fan). Hence $\epsilon_\eta$ is a positive integer, making this gap positive for $c\ge2$. There are only finitely many remaining inequalities. For example, any integer satisfying

$$
c>\max\left\{1,\ \max_{\substack{1\le i\le n\\j>n}}\frac{-\langle u_i,e_j\rangle}{\delta_j}\right\}
$$

works, with the inner maximum omitted when its index set is empty. The [toric ampleness criterion](../../../cartier-divisor.md#toric-ampleness-criterion) now gives

$$
\boxed{cD'-\tilde F\text{ is ample for every sufficiently large integer }c.}
$$

The new-ray assumption is essential to the printed construction. In dimension one, $\tilde e=e_1$ and the [fan subdivision](../../../toric-geometry.md#fan-subdivision) is unchanged, so the two purported distinct divisors coincide. If the displayed definition of $D'$ is applied literally on $\mathbb P^1$ with coefficients $a_1=-2$, $a_2=3$, then $D$ has degree one but $D'$ has degree $-1$, contradicting the conclusion. The argument above applies to the intended blowup in dimension at least two.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
