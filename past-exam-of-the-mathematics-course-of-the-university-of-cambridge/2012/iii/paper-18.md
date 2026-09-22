# Paper 18

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_18.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_18.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)

## 1

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $E=\mathbb C/\Lambda$, and let $\Lambda'$ be the inverse image of the [cyclic subgroup](../../../group.md#cyclic-subgroup) $G$ under the quotient map. Then $\Lambda\subset\Lambda'$ is an inclusion of [Euclidean lattices](../../../fourier-analysis.md#euclidean-lattice) with $\Lambda'/\Lambda\cong\mathbb Z/N\mathbb Z$. The [Smith normal form](../../../algebra.md#smith-normal-form) supplies a basis $u,v$ of $\Lambda'$ for which

$$
\Lambda=\mathbb Z(Nu)+\mathbb Zv.
$$

Choose the orientation of this basis so that $\operatorname{Im}(v/(Nu))>0$. Dividing the coordinate on $\mathbb C$ by $Nu$ gives an isomorphism of [complex tori](../../../complex-geometry.md#complex-torus)

$$
E\cong \mathbb C/(\mathbb Z+\mathbb Z\tau),\qquad \tau=\frac{v}{Nu}.
$$

Here $u$ maps to $1/N$, and its class generates $\Lambda'/\Lambda$. Thus the isomorphism carries $G$ to the required [cyclic subgroup](../../../group.md#cyclic-subgroup). **Every pair is represented: $\Phi$ is surjective.** This argument avoids assuming that an arbitrary integer lift of a primitive vector modulo $N$ is itself primitive.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Suppose $\tau_1=(a\tau_2+b)/(c\tau_2+d)$, with $ad-bc=1$, and put $\alpha=(c\tau_2+d)^{-1}$. The identities

$$
\alpha=a-c\tau_1,\qquad \alpha\tau_2=d\tau_1-b
$$

show that multiplication by $\alpha$ takes one [period lattice](../../../complex-analysis.md#period-lattice) isomorphically to the other: its basis matrix has determinant $ad-bc=1$. If $N\mid c$, the image of $1/N$ is congruent to $a/N$ modulo the target [period lattice](../../../complex-analysis.md#period-lattice). Moreover $ad\equiv1\pmod N$, so $a$ is a unit modulo $N$. The image therefore generates the same [cyclic subgroup](../../../group.md#cyclic-subgroup).

Conversely, a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) group isomorphism of [complex tori](../../../complex-geometry.md#complex-torus) lifts to $z\mapsto\alpha z$, with $\alpha\Lambda_{\tau_2}=\Lambda_{\tau_1}$. Indeed its lift fixing zero is additive: its failure to be additive is a continuous lattice-valued function, hence zero. An additive [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) map is complex linear. Write

$$
\alpha=a-c\tau_1,\qquad \alpha\tau_2=-b+d\tau_1.
$$

The corresponding integral basis matrix has determinant $1$: complex multiplication preserves the real orientation, and both bases $(1,\tau_j)$ are positively oriented. Solving gives $\tau_1=(a\tau_2+b)/(c\tau_2+d)$. Preservation of the [cyclic subgroup](../../../group.md#cyclic-subgroup) means $\alpha/N\equiv u/N\pmod{\Lambda_{\tau_1}}$ for some unit $u$ modulo $N$. Comparing the two real basis coefficients gives $N\mid c$. Thus the matrix lies in the [Gamma 0 congruence subgroup](../../../group-theory.md#gamma-0-congruence-subgroup), and **the classification is**

$$
\boxed{\mathcal E\cong\Gamma_0(N)\backslash\mathbb H.}
$$

This is the noncompact [modular curve](../../../modular-function.md#modular-curve) classification; no cusp points have been added.

## 2

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the convention that a [Hermitian form](../../../linear-algebra.md#hermitian-form) is complex linear in its first argument. In the [integral Hermitian forms on the square complex torus](../../../complex-geometry.md#integral-hermitian-forms-on-the-square-complex-torus) calculation, every [Hermitian form](../../../linear-algebra.md#hermitian-form) on $\mathbb C$ has the form $H_t(z,w)=t z\overline w$, where $t=H_t(1,1)$ is real. For $\lambda=m+ni$ and $\mu=r+si$ in the [period lattice](../../../complex-analysis.md#period-lattice),

$$
E_t(\lambda,\mu)=\operatorname{Im}H_t(\lambda,\mu)=t(nr-ms).
$$

Consequently integrality holds precisely when $t\in\mathbb Z$: necessity follows from $E_t(1,i)=-t$, and sufficiency follows from the displayed formula. Addition of [Hermitian forms](../../../linear-algebra.md#hermitian-form) corresponds to addition of $t$. Positivity is equivalent to $t>0$, since $H_t(z,z)=t|z|^2$. **The answer is**

$$
\boxed{H_t(z,w)=t z\overline w\quad(t\in\mathbb Z),\qquad H_t>0\iff t>0.}
$$

With the conjugate-linear-first convention the formula is $t\overline z w$ and the sign of $E_t$ reverses. The positive integer parameter is unchanged.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For the intended complex unit circle, put $u=\alpha(1)$ and $v=\alpha(i)$, with $|u|=|v|=1$. The complete family of [semicharacters of a complex lattice](../../../complex-geometry.md#semicharacter-of-a-complex-lattice) is

$$
\boxed{\alpha(m+ni)=(-1)^{mn}u^m v^n.}
$$

To obtain this, the identity at zero gives $\alpha(0)=1$; on each coordinate axis the alternating form vanishes, so $\alpha(m)=u^m$ and $\alpha(ni)=v^n$, also for negative integers. Combining the axes gives the factor $(-1)^{mn}$. Conversely, for $\lambda=m+ni$, $\mu=r+si$, the quotient of the proposed values is $(-1)^{ms+nr}$, which equals $e^{i\pi(nr-ms)}$. Hence every displayed formula is a [semicharacter of a complex lattice](../../../complex-geometry.md#semicharacter-of-a-complex-lattice) and none are missing.

The original PDF actually puts $z\in\mathbb Z$ in its definition of $C_1$. Under that literal reading $C_1=\{1,-1\}$, so **there are exactly four solutions**, given by the same formula with $u,v\in\{1,-1\}$. Under either reading the specified choice is $\alpha_1(m+ni)=(-1)^{mn}$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [Appell–Humbert theorem](../../../complex-geometry.md#appell-humbert-theorem) identifies the positive [Hermitian form](../../../linear-algebra.md#hermitian-form) $H_1$ with a [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle) whose [First Chern class](../../../complex-geometry.md#first-chern-class) is represented, in our linear-first convention, by

$$
\omega=\frac{i}{2}\,dz\wedge d\overline z=dx\wedge dy.
$$

Its integral over the square fundamental domain is $1$, so $\deg L=1$. In particular the oriented Chern pairing is $-E_1(1,i)=1$; using $E_1(1,i)$ without adjusting the Hermitian convention would give the wrong sign.

The [complex torus](../../../complex-geometry.md#complex-torus) has a nowhere-vanishing differential $dz$, so its [canonical divisor](../../../algebraic-geometry.md#canonical-divisor) is trivial and its genus is one. A nonzero section of a [line bundle](../../../ringed-space.md#line-bundle) of negative degree would have an [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) of negative degree, which is impossible. Thus $H^0(X,L^{-1})=0$. The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) and [Serre duality](../../../ringed-space.md#serre-duality) give

$$
h^0(X,L)-h^0(X,L^{-1})=\deg L=1.
$$

**Therefore $\boxed{h^0(X,L)=1}$.** The choice of [semicharacter of a complex lattice](../../../complex-geometry.md#semicharacter-of-a-complex-lattice) changes the degree-zero component of the [line bundle](../../../ringed-space.md#line-bundle), but not this calculation.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

A [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) group endomorphism of the [complex torus](../../../complex-geometry.md#complex-torus) lifts to multiplication by a scalar $c\in\mathbb C$, as in Question 1. It descends exactly when $c\Lambda\subseteq\Lambda$. Applying this condition to $1$ gives $c\in\mathbb Z[i]$. Conversely any [Gaussian integer](../../../commutative-algebra.md#gaussian-integer) $c$ preserves $\mathbb Z[i]$, since the latter is a ring. Addition of endomorphisms is addition of scalars, and composition is multiplication of scalars. **Thus, as rings,**

$$
\boxed{\operatorname{End}(X)\cong\mathbb Z[i].}
$$

The wording “endomorphism algebra” here denotes this integral [endomorphism ring of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve). If it instead meant the rational algebra $\operatorname{End}^0(X)=\operatorname{End}(X)\otimes_{\mathbb Z}\mathbb Q$, that algebra would be $\mathbb Q(i)$.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Pulling back the factors of automorphy in the [Appell–Humbert theorem](../../../complex-geometry.md#appell-humbert-theorem) by $z\mapsto cz$, where $c=a+bi$, pulls back both the [Hermitian form](../../../linear-algebra.md#hermitian-form) and the [semicharacter of a complex lattice](../../../complex-geometry.md#semicharacter-of-a-complex-lattice). Thus **the explicit answer is**

$$
\boxed{H(z,w)=(a^2+b^2)z\overline w,\qquad \alpha(\lambda)=\alpha_1((a+bi)\lambda).}
$$

Writing $\lambda=m+ni$ makes the second formula completely explicit:

$$
\alpha(m+ni)=(-1)^{(am-bn)(bm+an)}=(-1)^{ab(m+n)+(a^2+b^2)mn}.
$$

The second equality is an equality of signs, obtained by reducing the exponents modulo $2$. The [Hermitian form](../../../linear-algebra.md#hermitian-form) follows from $H_1(cz,cw)=|c|^2H_1(z,w)$. Its integer parameter equals the norm of the [Gaussian integer](../../../commutative-algebra.md#gaussian-integer), agreeing with the degree of this nonzero [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves). The formulas also include $c=0$, when the pulled-back [line bundle](../../../ringed-space.md#line-bundle) is trivial.

## 3

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The bundle is on $A$, so the printed, undefined target $\operatorname{Pic}(X)$ must be read as the [Picard group](../../../ringed-space.md#picard-group) $\operatorname{Pic}(A)$. Write this [Picard group](../../../ringed-space.md#picard-group) additively and set $q(h)=[h^*L]$. The zero morphism pulls back $L$ to a constant one-dimensional vector space tensored with $\mathcal O_A$, so $q(0)=0$. The [Theorem of the Cube](../../../abelian-variety.md#theorem-of-the-cube), pulled back along $(f,g,h):A\to B^3$, gives

$$
q(f+g+h)-q(f+g)-q(f+h)-q(g+h)+q(f)+q(g)+q(h)=0.
$$

This is the [bilinear cross-effect of a line bundle on an abelian variety](../../../abelian-variety.md#bilinear-cross-effect-of-a-line-bundle-on-an-abelian-variety): set $d(f,g)=q(f+g)-q(f)-q(g)$. Substitution into this identity gives

$$
d(f+g,h)=d(f,h)+d(g,h).
$$

The definition gives $d(f,g)=d(g,f)$, so additivity holds in both arguments. Additivity includes negative multiples and the zero morphism. **Hence $D_L$ is a symmetric [bilinear map](../../../linear-algebra.md#bilinear-map) with values in $\operatorname{Pic}(A)$.** The equalities refer to isomorphism classes of [line bundles](../../../ringed-space.md#line-bundle); without chosen rigidifications they are not asserted to be specified canonical isomorphisms of bundles.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $m:B\times B\to B$ be addition, and let $p_1,p_2$ be the projections. Consider the [line bundle](../../../ringed-space.md#line-bundle)

$$
M=m^*L\otimes p_1^*L^{-1}\otimes p_2^*L^{-1}.
$$

Its restriction to $B\times\{y\}$ has [Picard group](../../../ringed-space.md#picard-group) class $[T_y^*L\otimes L^{-1}]=\phi_L(y)$; the factor $L_y^{-1}$ is a constant line and has trivial class. Its restriction to $\{0\}\times B$ is also trivial. Choose a trivialization of the fiber $L_0$ and use it to normalize along the zero sections. The defining universal property of the normalized [Poincaré line bundle](../../../abelian-variety.md#poincare-line-bundle) then identifies

$$
M\cong(\operatorname{id}_B,\phi_L)^*P_B.
$$

More explicitly, both sides have the same restrictions to all fibers of the second projection, and both are normalized on $\{0\}\times B$; the [Seesaw theorem](../../../abelian-variety.md#seesaw-theorem) makes their quotient trivial. Here $\phi_L:B\to\widehat B$ is the [homomorphism associated to a line bundle on an abelian variety](../../../abelian-variety.md#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety), and $\widehat B$ is the [dual abelian variety](../../../abelian-variety.md#dual-abelian-variety). Pull back by $(f,g)$ to obtain **the required identity**

$$
\boxed{D_L(f,g)\cong(f,\phi_L\circ g)^*P_B.}
$$

The choice of fiber trivialization is immaterial to this identity in the [Picard group](../../../ringed-space.md#picard-group).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For $M\in\operatorname{Pic}^0(B)$, translations preserve its [line bundle](../../../ringed-space.md#line-bundle) class, so $\phi_M=0$. Equivalently, the kernel of $L\mapsto\phi_L$ is the [Identity component of the Picard group](../../../abelian-variety.md#identity-component-of-the-picard-group). Applying the preceding [Poincaré line bundle](../../../abelian-variety.md#poincare-line-bundle) formula to $M$ yields

$$
D_M(f,g)\cong(f,0)^*P_B\cong\mathcal O_A,
$$

since the normalized [Poincaré line bundle](../../../abelian-variety.md#poincare-line-bundle) is trivial on $B\times\{0\}$. Pullback and [tensor products of sheaves](../../../ringed-space.md#tensor-product-of-sheaves) also give $D_{L\otimes M}=D_L\otimes D_M$. **Thus $D_L$ depends only on $[L]\in\boxed{\operatorname{NS}(B)}$, the [Néron-Severi group](../../../ringed-space.md#neron-severi-group).**

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For a [group homomorphism](../../../group-theory.md#group-homomorphism) $h:A\to B$, the dual morphism $\widehat h:\widehat B\to\widehat A$ is pullback of algebraically trivial [line bundles](../../../ringed-space.md#line-bundle). Translations satisfy $h\circ T_x=T_{h(x)}\circ h$, and therefore

$$
\phi_{h^*L}(x)=h^*(T_{h(x)}^*L\otimes L^{-1})=(\widehat h\circ\phi_L\circ h)(x).
$$

Also $\phi_{L\otimes M}=\phi_L+\phi_M$ and $\phi_{L^{-1}}=-\phi_L$. Dualizing is additive: $\widehat{f+g}=\widehat f+\widehat g$, since algebraically trivial [line bundles](../../../ringed-space.md#line-bundle) obey the [Theorem of the square](../../../abelian-variety.md#theorem-of-the-square). Apply these identities to the three factors defining $D_L$. The two diagonal terms cancel in the expansion

$$
\begin{aligned}
\phi_{D_L(f,g)}&=(\widehat f+\widehat g)\phi_L(f+g)-\widehat f\phi_Lf-\widehat g\phi_Lg\\
&=\widehat f\phi_Lg+\widehat g\phi_Lf.
\end{aligned}
$$

**Hence $\boxed{\phi_{D_L(f,g)}=\widehat f\circ\phi_L\circ g+\widehat g\circ\phi_L\circ f}$.**

## 4

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For a [line bundle](../../../ringed-space.md#line-bundle) $M$ on $C\times T$, put $d(t)=\deg M_t$, and choose an [ample line bundle](../../../ringed-space.md#ample-line-bundle) $A$ on $C$. Fix $t_0$. For sufficiently large $q$, both $H^1(C,M_{t_0}\otimes A^q)$ and $H^1(C,M_{t_0}^{-1}\otimes A^q)$ vanish, by [Serre duality](../../../ringed-space.md#serre-duality) and negativity of the degrees of their dual canonical twists. The [semicontinuity theorem for coherent cohomology](../../../ringed-space.md#semicontinuity-theorem-for-coherent-cohomology) makes both groups vanish on a neighborhood of $t_0$. The family is flat over $T$: $C\times T\to T$ is flat and the sheaves in question are locally free.

On that neighborhood the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives

$$
h^0(C,M_t\otimes A^q)=d(t)+q\deg A+1-g,\qquad h^0(C,M_t^{-1}\otimes A^q)=-d(t)+q\deg A+1-g.
$$

Upper semicontinuity of both zeroth [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) dimensions, after shrinking again, gives $d(t)\leq d(t_0)$ and $-d(t)\leq-d(t_0)$. Hence $d(t)=d(t_0)$. **The degree is locally constant, and thus constant on connected $T$.** With the usual convention that a variety is irreducible, this proves the assertion as printed. If disconnected varieties are allowed, the necessary qualification is constancy on each connected component: take $T$ to be two points and the bundles $\mathcal O_{\mathbb P^1}$ and $\mathcal O_{\mathbb P^1}(1)$ to see that a global constant degree need not exist.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Pull $L$ back by the [morphism of varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties)

$$
a:C\times X\longrightarrow X,\qquad (c,x)\longmapsto\varphi(c)+x.
$$

The fiber of this [line bundle](../../../ringed-space.md#line-bundle) over $x$ is $\varphi^*T_x^*L$. An [abelian variety](../../../abelian-variety.md) is connected, so the preceding [constancy of line bundle degree in a family](../../../ringed-space.md#constancy-of-line-bundle-degree-in-a-family) applies. **Consequently $\boxed{\deg(\varphi^*T_x^*L)=\deg(\varphi^*L)}$ for every $x\in X$.**

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The defining section of $\mathcal O_X(D)$ is nowhere zero on $C$, so its restriction is trivial and has degree zero. Every translated [line bundle](../../../ringed-space.md#line-bundle) also has degree zero on $C$, by the preceding part. For any $t\in X$, either $C\subseteq D-t$ or the defining section of $T_t^*\mathcal O_X(D)$ restricts to a nonzero section on $C$. In the second case its zero [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) has degree zero, so it has no zeros. Thus **a translate of $D$ either contains all of $C$ or misses all of $C$.**

Take $d\in D$ and $x_1,x_2\in C$. The translate $D-(d-x_1)$ contains $x_1$, hence all of $C$. In particular $d+(x_2-x_1)\in D$. This proves $D+(x_2-x_1)\subseteq D$; exchanging $x_1,x_2$ proves the reverse inclusion. Since the prime [Weil divisor](../../../algebraic-geometry.md#weil-divisor) $D$ is reduced and translation is an automorphism, equality of these sets gives equality of [Weil divisors](../../../algebraic-geometry.md#weil-divisor). Remembering that pullback by $T_t$ translates the divisor by $-t$, **the answer is**

$$
\boxed{T_{x_1-x_2}^*D=D.}
$$

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

The [line bundle translation stabilizer](../../../abelian-variety.md#line-bundle-translation-stabilizer) is the closed subgroup

$$
K(L)=\ker\phi_L=\{x\in X:T_x^*L\cong L\}.
$$

Each difference $x_1-x_2$ lies in $K(L)$, by the equality of [Weil divisors](../../../algebraic-geometry.md#weil-divisor) just proved. Thus the subgroup they generate lies in $K(L)$, and closedness puts its [Zariski topology](../../../algebraic-geometry.md#zariski-topology) closure there too. **Therefore $\boxed{Y\subseteq K(L)}$.** The closure of a subgroup is again a subgroup: multiplication and inversion preserve its closure by continuity. In this setting it is connected as well, since $C-C$ is connected and contains zero, and the increasing finite sums of $C-C$ are connected with a common point. Its reduced closure is an abelian subvariety.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

For the [curve generation criterion for an abelian variety](../../../abelian-variety.md#curve-generation-criterion-for-an-abelian-variety), first suppose $Y=X$ and an irreducible [Weil divisor](../../../algebraic-geometry.md#weil-divisor) $D$ avoids $C$. The preceding part gives $K(\mathcal O_X(D))=X$, so $\phi_{\mathcal O_X(D)}=0$ and $\mathcal O_X(D)\in\operatorname{Pic}^0(X)$. A nonzero [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) cannot have this property: if $H$ is an [ample line bundle](../../../ringed-space.md#ample-line-bundle) and $g=\dim X$, then the [intersection product of Cartier divisors](../../../algebraic-geometry.md#intersection-product-of-cartier-divisors) $D\cdot H^{g-1}$ is positive, whereas an algebraically trivial [line bundle](../../../ringed-space.md#line-bundle) has zero intersection with every curve. The latter follows from constancy of degree along a connected family defining algebraic equivalence; the former is the positive projective degree of $D$ after replacing $H$ by a very ample power. This contradiction proves that $C$ meets every irreducible [Weil divisor](../../../algebraic-geometry.md#weil-divisor).

Conversely suppose $Y\ne X$. Fix $c_0\in C$, so $C\subseteq c_0+Y$. Use the permitted fiber theorem to choose a [morphism of varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties) $f:X\to Z$ with $f^{-1}(z_0)=Y$. This morphism is nonconstant because $Y$ is proper. Choose an affine neighborhood $U$ of $z_0$. The irreducible image $f(X)$ has positive dimension, so its intersection with $U$ does too; some regular function $h$ on $U$ is nonconstant on this intersection. Then $F=h\circ f$ is a nonconstant rational function on $X$, regular on $f^{-1}(U)$.

The [pole divisor avoiding a fiber](../../../projective-space.md#pole-divisor-avoiding-a-fiber) construction applies: its pole [Weil divisor](../../../algebraic-geometry.md#weil-divisor) is nonzero. Indeed on the smooth, hence normal, [projective variety](../../../projective-space.md#projective-variety) $X$, a rational function with no codimension-one poles extends to a global regular function; every global regular function on a connected [projective variety](../../../projective-space.md#projective-variety) is constant. Every pole component $D_0$ lies outside $f^{-1}(U)$ and hence avoids $Y$. Therefore $D_0+c_0$ is an irreducible [Weil divisor](../../../algebraic-geometry.md#weil-divisor) disjoint from $c_0+Y$, and in particular from $C$. This proves the converse using precisely the fiber fact allowed in the question, without requiring a projective target $Z$. **The criterion is**

$$
\boxed{Y=X\quad\Longleftrightarrow\quad C\text{ meets every irreducible divisor of }X.}
$$

## 5

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Write the [projective plane](../../../projective-space.md#projective-plane) as $\mathbb P(V)$ for a three-dimensional complex vector space $V$. A projective line is the zero set of a nonzero linear functional $\ell\in V^*$. Two such functionals give the same line exactly when they differ by a nonzero scalar. Hence the parameter space of lines is the [dual projective space](../../../projective-space.md#dual-projective-space) $\mathbb P(V^*)$. A choice of basis identifies $V^*$ with $\mathbb C^3$, giving **$\boxed{(\mathbb P^2)^\vee\cong\mathbb P^2}$.** The description as $\mathbb P(V^*)$ is intrinsic; the identification with the original $\mathbb P(V)$ requires a choice.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Represent the [smooth plane conic](../../../algebraic-geometry.md#smooth-plane-conic) by $v^{\mathsf T}Qv=0$, with $Q$ an invertible symmetric $3\times3$ matrix. The tangent line at $[v]$ has coefficients $\ell=Qv$, because the differential is $2v^{\mathsf T}Q$. Thus its image in the [dual projective space](../../../projective-space.md#dual-projective-space) satisfies

$$
\ell^{\mathsf T}Q^{-1}\ell=0.
$$

Conversely any nonzero $\ell$ satisfying this equation gives $v=Q^{-1}\ell$, a point of the original [smooth plane conic](../../../algebraic-geometry.md#smooth-plane-conic) whose tangent is $[\ell]$. This correspondence is the restriction of an invertible projective linear transformation. **The [dual conic](../../../algebraic-geometry.md#dual-conic) is therefore the smooth conic**

$$
\boxed{C_1^\vee:\ell^{\mathsf T}Q^{-1}\ell=0.}
$$

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

To analyze the [genus one tangent incidence curve of two conics](../../../algebraic-geometry.md#genus-one-tangent-incidence-curve-of-two-conics), choose projective coordinates in which $C_1$ has equation $XZ-Y^2=0$. Its points and tangent lines are parametrized by $[a:b]\in\mathbb P^1$ as

$$
[a^2:ab:b^2],\qquad \ell_{[a:b]}:\ b^2X-2abY+a^2Z=0.
$$

For $x=[X:Y:Z]\in C_2$, the incidence equation is a nonzero homogeneous quadratic in $a,b$, so the projection $E\to C_2$ is finite of degree two. Its discriminant vanishes exactly when $Y^2-XZ=0$, that is, at $C_1\cap C_2$. There are four such points; [Bézout theorem](../../../algebraic-geometry.md#bezout-s-theorem) says their intersection multiplicities sum to four, so all four intersections are transverse.

Locally on $C_2$, after choosing an affine tangent-parameter chart and completing the square, the incidence equation is $w^2=u(s)$, where $s$ is a local parameter and $u$ has a simple zero at each intersection. This is smooth, with ramification index two there; away from those points the roots are distinct and the cover is étale. The analogous chart covers a root at infinity. Thus $E$ is smooth everywhere, and **the cover has exactly four ramification points**. It is connected: the discriminant has odd valuation at each of its four zeros, so it cannot be a square in the function field of $C_2$. The associated quadratic extension is therefore a field, not two separate sheets.

A [smooth plane conic](../../../algebraic-geometry.md#smooth-plane-conic) over $\mathbb C$ is isomorphic to the [projective line](../../../finite-group-theory.md#projective-line). Apply the [Riemann-Hurwitz formula](../../../complex-analysis.md#riemann-hurwitz-formula) to this connected degree-two cover:

$$
2g(E)-2=2(2\cdot0-2)+4=0.
$$

**Consequently $\boxed{g(E)=1}$, and $E$ is a smooth projective [genus one curve](../../../normalization-of-an-algebraic-curve.md#genus-one-curve).**

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

The printed construction is not well defined: the next tangent must pass through $x_1$, rather than $x_0$. If $x_0\ne x_1$ and $\ell_1\ne\ell_0$, a second line through $x_0$ cannot also pass through $x_1$, because the unique line through both points is $\ell_0$. Here is a concrete counterexample satisfying all the conic hypotheses. In the affine chart take

$$
C_1:x^2+y^2=1,\qquad C_2:x^2/4+y^2/9=1,
$$

with $\ell_0:x=1$, $x_0=(1,3\sqrt3/2)$ and $x_1=(1,-3\sqrt3/2)$. The second tangent through $x_0$ is $-23x+12\sqrt3y=31$. It does not contain $x_1$: its left side there is $-77$. The conics meet transversely at the four complex points with $x^2=32/5$, $y^2=-27/5$. Thus this is a defect in the original PDF, not just in its conversion.

For the corrected construction, let $\iota_\ell$ exchange the two points of $C_2$ on a fixed tangent line, and let $\iota_x$ exchange the two tangents to $C_1$ through a fixed point of $C_2$. Both projections from $E$ are degree-two morphisms to a [smooth plane conic](../../../algebraic-geometry.md#smooth-plane-conic): for the line projection this follows from intersecting a line with $C_2$, which has no line component. Since $E$ is smooth and the ground field has characteristic zero, their quadratic function-field extensions define regular involutions on the whole curve. At a ramification point “the second” point is the same point, counted with multiplicity. Each switch is an [involution of a degree-two map from a genus one curve](../../../normalization-of-an-algebraic-curve.md#involution-of-a-degree-two-map-from-a-genus-one-curve). Hence the corrected step is the everywhere-defined automorphism $F=\iota_x\circ\iota_\ell$.

Choose an origin $O$ on the [genus one curve](../../../normalization-of-an-algebraic-curve.md#genus-one-curve). The [Abel-Jacobi map of a genus-one curve](../../../normalization-of-an-algebraic-curve.md#abel-jacobi-map-of-a-genus-one-curve) identifies $E$ with $\operatorname{Pic}^0(E)$ by $p\mapsto\mathcal O_E(p-O)$. Fibers of each degree-two projection are linearly equivalent [Weil divisors](../../../algebraic-geometry.md#weil-divisor), since they are pullbacks of points of $\mathbb P^1$. Thus their group sums are constant: for suitable $a,b\in E$,

$$
\iota_\ell(p)=a-p,\qquad \iota_x(p)=b-p,\qquad F(p)=p+(b-a).
$$

This also holds at the ramification points, where $2p=a$ or $2p=b$. Therefore the corrected step is a [translation on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#translation-on-an-elliptic-curve). If $F^n(p_0)=p_0$ for one point, then $n(b-a)=0$. It follows that $F^n(p)=p$ for every $p\in E$. **The corrected construction has the [Poncelet porism](../../../algebraic-geometry.md#poncelet-porism): one periodic orbit implies all orbits are periodic, with the same least period.** The literal printed construction fails before this conclusion; the proof establishes the intended, explicitly corrected assertion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
