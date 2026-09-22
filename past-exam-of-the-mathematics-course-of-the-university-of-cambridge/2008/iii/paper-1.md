# Paper 1

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper1.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper1.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
  - [d](#8/d)
    - [Solution](#8/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use complex [inner products](../../../linear-algebra.md#inner-product) linear in the first argument throughout. The [spectral theorem for compact self-adjoint operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) states that, for a [compact operator](../../../compact-operator.md) $T=T^*$ on a [Hilbert space](../../../hilbert-space.md), its nonzero spectral values are real [eigenvalues](../../../linear-operator-theory.md#eigenvalue), each of finite multiplicity, with no possible accumulation point except zero. Moreover,

$$
\boxed{H=\ker T\oplus\bigoplus_{\lambda\ne0}\ker(T-\lambda I),
\qquad T=\sum_{\lambda\ne0}\lambda P_\lambda,}
$$

where $P_\lambda$ are the mutually orthogonal [eigenspace](../../../linear-operator-theory.md#eigenspace) [projections](../../../vector-space.md#projection-linear-algebra). The operator series converges in [operator norm](../../../continuous-dual-space.md#operator-norm) when the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are listed in decreasing absolute value. The sum is at most countable, even if the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is nonseparable. Zero need not be an [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

First prove that a nonzero compact [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) has an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of magnitude its [norm](../../../functional-analysis.md#norm), without assuming a spectral decomposition. Put $r=\|T\|>0$ and choose unit [vectors](../../../vector-space.md#vector) $\xi_n$ with $\|T\xi_n\|\to r$. Since $\|T^2\xi\|\leq r\|T\xi\|$, expansion gives

$$
\|(T^2-r^2I)\xi_n\|^2
\leq r^2\bigl(r^2-\|T\xi_n\|^2\bigr)\longrightarrow0.
$$

[Compactness](../../../topology.md#compact-space) of $T^2$ supplies a subsequence for which $T^2\xi_n$ converges; the displayed estimate then forces $\xi_n$ itself to converge to a unit [vector](../../../vector-space.md#vector) $\xi$ satisfying $T^2\xi=r^2\xi$. The [vectors](../../../vector-space.md#vector) $\xi+T\xi/r$ and $\xi-T\xi/r$ are [eigenvectors](../../../linear-operator-theory.md#eigenvector) for $r$ and $-r$, respectively, whenever nonzero, and they cannot both vanish. This proves the claim.

Self-adjointness gives reality of every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of [eigenspaces](../../../linear-operator-theory.md#eigenspace) for distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue). An [eigenspace](../../../linear-operator-theory.md#eigenspace) for $\lambda\ne0$ cannot contain an infinite orthonormal sequence: its images under $T$ would have pairwise distance $\sqrt2|\lambda|$, contradicting [compactness](../../../topology.md#compact-space). The same argument proves that there are only finitely many mutually orthogonal [eigenvectors](../../../linear-operator-theory.md#eigenvector) with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of magnitude at least any given $\varepsilon>0$. Hence all nonzero [eigenspaces](../../../linear-operator-theory.md#eigenspace) together have a countable [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), and their [eigenvalues](../../../linear-operator-theory.md#eigenvalue) tend to zero if there are infinitely many.

Let $K$ be the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of the closed span of all these [eigenspaces](../../../linear-operator-theory.md#eigenspace). It is invariant under $T$. If $T|_K$ were nonzero, the norm-attaining [eigenvalue](../../../linear-operator-theory.md#eigenvalue) argument applied to that compact [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) restriction would produce another nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector), a contradiction. Thus $K\subseteq\ker T$, and the converse inclusion follows from [orthogonality](../../../linear-algebra.md#orthogonal-vectors). This establishes the asserted decomposition. On its orthogonal summands the tail of the operator series has [norm](../../../functional-analysis.md#norm) equal to the supremum of the omitted [eigenvalue](../../../linear-operator-theory.md#eigenvalue) magnitudes, proving [norm](../../../functional-analysis.md#norm) convergence.

Finally, a nonzero complex number not among these [eigenvalues](../../../linear-operator-theory.md#eigenvalue) has positive distance from their set and from zero. Inverting $T-zI$ separately on the [eigenspaces](../../../linear-operator-theory.md#eigenspace) and [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) therefore gives a bounded inverse. This proves that no other nonzero spectral values occur and completes the theorem.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a [finite-rank operator](../../../compact-operator.md#finite-rank-operator) $T$, define $|T|=(T^*T)^{1/2}$ and its [trace norm](../../../functional-analysis.md#trace-norm) by

$$
\boxed{\|T\|_1=\operatorname{Tr}|T|=\sum_{j=1}^r s_j,}
$$

where $s_j>0$ are its nonzero [singular values](../../../linear-algebra.md#singular-value), counted with multiplicity. The finite-rank spectral theorem gives orthonormal systems $(u_j),(v_j)$ with $T=\sum_js_jR_{u_j,v_j}$, where $R_{x,y}z=\langle z,y\rangle x$.

For every [bounded operator](../../../topological-vector-space.md#continuous-linear-operator) $B$,

$$
\operatorname{Tr}(BT)=\sum_js_j\langle Bu_j,v_j\rangle,
\qquad |\operatorname{Tr}(BT)|\leq\|B\|\sum_js_j.
$$

Choose the contraction $B$ taking $u_j$ to $v_j$ and vanishing on their [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). It attains equality, so

$$
\boxed{\|T\|_1=\sup_{\|B\|\leq1}|\operatorname{Tr}(BT)|.}
$$

This formula proves the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and absolute homogeneity. Also $\|T\|\leq\|T\|_1$, so vanishing of the [trace norm](../../../functional-analysis.md#trace-norm) forces $T=0$. Thus it is a [norm](../../../functional-analysis.md#norm) on the [vector](../../../vector-space.md#vector) space of [finite-rank operators](../../../compact-operator.md#finite-rank-operator).

The map $B\mapsto F_B$, where $F_B(T)=\operatorname{Tr}(BT)$, is a bounded linear map into the dual of this normed space. Its [norm](../../../functional-analysis.md#norm) is at most $\|B\|$. Rank-one tests give the reverse inequality: $\|R_{x,y}\|_1=\|x\|\|y\|$ and $F_B(R_{x,y})=\langle Bx,y\rangle$, so taking unit [vectors](../../../vector-space.md#vector) $x,y$ gives $\|F_B\|=\|B\|$.

Conversely, let $F$ be a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) for the [trace norm](../../../functional-analysis.md#trace-norm). The [sesquilinear form](../../../linear-algebra.md#sesquilinear-form) $\beta(x,y)=F(R_{x,y})$ satisfies

$$
|\beta(x,y)|\leq\|F\|\|x\|\|y\|.
$$

The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) gives a unique [bounded operator](../../../topological-vector-space.md#continuous-linear-operator) $B$ with $\beta(x,y)=\langle Bx,y\rangle$, and $\|B\|\leq\|F\|$. Since every [finite-rank operator](../../../compact-operator.md#finite-rank-operator) is a finite sum of [rank-one operators](../../../compact-operator.md#rank-one-operator), [linearity](../../../vector-space.md#linearity) implies $F(T)=\operatorname{Tr}(BT)$ for every $T$. Hence

$$
\boxed{(\mathcal F(H),\|\cdot\|_1)^*\cong B(H)\text{ isometrically}.}
$$

The same identification extends to the completion, the [trace-class operators](../../../compact-operator.md#trace-class-operator). This is [trace-class duality](../../../compact-operator.md#trace-class-duality); completeness of the original finite-rank space is not required to identify its bounded dual.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_i)$, define the [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm) by $\|T\|_2^2=\sum_i\|Te_i\|^2$. For a possibly uncountable [basis](../../../vector-space.md#basis), the nonnegative sum means the supremum over finite subsets. [Parseval's identity](../../../fourier-analysis.md#parseval-identity) gives, for any other [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(f_j)$,

$$
\sum_i\|Te_i\|^2=\sum_{i,j}|\langle Te_i,f_j\rangle|^2
=\sum_j\|T^*f_j\|^2.
$$

Changing the domain [basis](../../../vector-space.md#basis) in the last expression proves [basis](../../../vector-space.md#basis) independence. Polarization gives a basis-independent [inner product](../../../linear-algebra.md#inner-product)

$$
\boxed{\langle T,S\rangle_2=\sum_i\langle Te_i,Se_i\rangle
=\operatorname{Tr}(S^*T),}
$$

with the same first-argument linear convention. The sums converge by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). The operator-norm bound $\|T\|\leq\|T\|_2$ follows by applying Cauchy-Schwarz to the coordinates of a unit [vector](../../../vector-space.md#vector).

To prove completeness, let $(T_n)$ be Cauchy in this [norm](../../../functional-analysis.md#norm). The operator-norm bound gives a bounded-operator limit $T$. For a finite subset $F$ of the [basis](../../../vector-space.md#basis),

$$
\sum_{i\in F}\|(T_n-T)e_i\|^2
=\lim_{m\to\infty}\sum_{i\in F}\|(T_n-T_m)e_i\|^2.
$$

For large $n$, the right side is uniformly small by the Cauchy property. Taking the supremum over $F$ shows $T_n-T$ is [Hilbert-Schmidt](../../../compact-operator.md#hilbert-schmidt-operator) and $\|T_n-T\|_2\to0$; it also shows $T$ is [Hilbert-Schmidt](../../../compact-operator.md#hilbert-schmidt-operator). Thus **the [Hilbert-Schmidt operators](../../../compact-operator.md#hilbert-schmidt-operator) form a [Hilbert space](../../../hilbert-space.md)**. [Finite-rank operators](../../../compact-operator.md#finite-rank-operator) are dense there: keeping finitely many [basis](../../../vector-space.md#basis) columns makes the sum of omitted squared column [norms](../../../functional-analysis.md#norm) tend to zero. The operator-norm bound then shows that every [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator) is compact.

Now let $U$ be a strongly continuous [unitary representation](../../../representation-theory.md#unitary-representation) of the compact metric [group](../../../group.md) $G$, as is standard for a representation of a topological [group](../../../group.md). Fix $\xi\ne0$ and average the positive [rank-one operator](../../../compact-operator.md#rank-one-operator) $R_{\xi,\xi}$:

$$
K=\int_G U_gR_{\xi,\xi}U_g^*\,dg.
$$

The integrand is continuous in the [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm), so this [Bochner integral](../../../measure-theory.md#bochner-integral) exists in the complete space just proved. Normalized [Haar measure](../../../measure-theory.md#haar-measure) and invariance show that $K$ is positive, compact and commutes with every $U_g$. Moreover,

$$
\langle K\xi,\xi\rangle=\int_G|\langle U_g\xi,\xi\rangle|^2\,dg>0:
$$

the integrand is positive near the identity and every nonempty open set has positive [Haar measure](../../../measure-theory.md#haar-measure). Thus $K\ne0$. A nonzero [eigenspace](../../../linear-operator-theory.md#eigenspace) is finite-dimensional and invariant under $U$, by (a). Within it choose a nonzero [invariant subspace](../../../representation-theory.md#invariant-subspace) of smallest dimension; it is irreducible. Its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) is invariant because the representation is unitary, so the finite-dimensional space splits into irreducibles.

Take a maximal orthogonal family of such finite-dimensional irreducible [invariant subspaces](../../../representation-theory.md#invariant-subspace). If their closed span had a nonzero [orthogonal complement](../../../hilbert-space.md#orthogonal-complement), the same averaging argument on that complement would produce another member, contradicting maximality. Therefore

$$
\boxed{H=\bigoplus_\alpha H_\alpha,
\quad\dim H_\alpha<\infty,\quad U|_{H_\alpha}\text{ irreducible}.}
$$

This [compact averaging of a rank-one operator](../../../compact-operator.md#compact-averaging-of-a-rank-one-operator) argument does not require $H$ itself to be separable. Strong [continuity](../../../calculus.md#continuous-function) is the topological representation hypothesis used in the averaging step.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [Hadamard space](../../../geometric-group-theory.md#hadamard-space) is a complete [CAT(0) space](../../../geometric-group-theory.md#cat-0-space). A useful equivalent definition, which makes the remaining assertions consequences rather than assumptions, is a [complete metric space](../../../topological-analysis.md#complete-metric-space) in which every pair $x,y$ has a midpoint $m$, with $d(x,m)=d(y,m)=d(x,y)/2$, satisfying

$$
\boxed{d(z,m)^2\leq\frac12d(z,x)^2+\frac12d(z,y)^2-\frac14d(x,y)^2
\quad\text{for every }z.}
$$

This is the nonpositive-curvature midpoint inequality. Euclidean [Hilbert spaces](../../../hilbert-space.md) satisfy it with equality in the parallelogram formula. The comparison argument in (c) shows that this definition gives the usual CAT(0) triangle condition.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $L=d(x,y)$. If $m'$ is any other metric midpoint, apply the inequality from (a) to the chosen midpoint $m$ with $z=m'$. The right side is $\tfrac12(L/2)^2+\tfrac12(L/2)^2-L^2/4=0$, so $m=m'$. **Every pair has a unique midpoint.**

Choose successive midpoints to define $\gamma(k/2^n)$ on all dyadic parameters. Consecutive points at level $n$ have distance $L/2^n$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $d(\gamma(s),\gamma(t))\leq(t-s)L$ for dyadic $s<t$. Conversely,

$$
L\leq d(x,\gamma(s))+d(\gamma(s),\gamma(t))+d(\gamma(t),y)
\leq sL+d(\gamma(s),\gamma(t))+(1-t)L,
$$

which gives the reverse bound. Thus equality holds. Completeness extends this map uniquely and continuously to $[0,1]$, retaining $d(\gamma(s),\gamma(t))=|s-t|L$. It is a constant-speed [geodesic](../../../riemannian-geometry.md#geodesic).

Every other [geodesic](../../../riemannian-geometry.md#geodesic) has the same midpoint, and then the same successive midpoints, so agrees on all dyadic parameters. [Continuity](../../../calculus.md#continuous-function) gives agreement everywhere. Hence $\boxed{\text{there is exactly one geodesic segment between any two points}.}$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The comparison triangle must have third side $d(x,y)$: the printed $d(y,z)$ contains an undefined $z$. Use $A=d(a,x)$, $B=d(a,y)$ and $C=d(x,y)$.

First extend the midpoint inequality along any constant-speed [geodesic](../../../riemannian-geometry.md#geodesic) $\gamma$ from $p$ to $q$. If $L=d(p,q)$, the function $d(z,\gamma(t))^2-L^2t^2$ is midpoint-convex by (a). Iteration proves its convexity bound for dyadic $t$, and [continuity](../../../calculus.md#continuous-function) then gives the [Hadamard squared-distance inequality](../../../geometric-group-theory.md#hadamard-squared-distance-inequality)

$$
d(z,\gamma(t))^2\leq(1-t)d(z,p)^2+td(z,q)^2-t(1-t)L^2.
$$

Apply this first to $[a,x]$ with $z=y_t$, and then to $[a,y]$ with $z=x$:

$$
d(x_s,y_t)^2\leq(1-s)t^2B^2+s\bigl[(1-t)A^2+tC^2-t(1-t)B^2\bigr]
-s(1-s)A^2.
$$

Simplification gives

$$
\boxed{d(x_s,y_t)^2\leq s^2A^2+t^2B^2-st(A^2+B^2-C^2).}
$$

In a Euclidean comparison triangle, the cosine rule gives the scalar product of the two [vectors](../../../vector-space.md#vector) from the common vertex as $(A^2+B^2-C^2)/2$. The squared distance between their multiples $s$ and $t$ is exactly the right side displayed above. Taking nonnegative square roots proves the required triangle comparison, including degenerate Euclidean triangles.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $p,q$ lie in the [closed ball](../../../topological-analysis.md#closed-ball) of center $z$ and radius $R$. On their unique [geodesic](../../../riemannian-geometry.md#geodesic), the [Hadamard squared-distance inequality](../../../geometric-group-theory.md#hadamard-squared-distance-inequality) gives

$$
d(z,\gamma(t))^2\leq(1-t)d(z,p)^2+td(z,q)^2-t(1-t)d(p,q)^2
\leq R^2.
$$

Thus every point of that [geodesic](../../../riemannian-geometry.md#geodesic) lies in the ball. By uniqueness there are no other [geodesics](../../../riemannian-geometry.md#geodesic) to consider, so **every [closed ball](../../../topological-analysis.md#closed-ball) is geodesically convex**.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Stone theorem for the circle group](../../../representation-theory.md#stone-theorem-for-the-circle-group) says that a strongly continuous [unitary representation](../../../representation-theory.md#unitary-representation) $U$ of $\mathbb T=\{z:|z|=1\}$ has an orthogonal decomposition

$$
\boxed{H=\bigoplus_{n\in\mathbb Z}H_n,\qquad U_z|_{H_n}=z^nI.}
$$

Equivalently, $U_z=\sum_nz^nP_n$ strongly, with mutually [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) $P_n$ summing strongly to the identity. Define these [projections](../../../vector-space.md#projection-linear-algebra) using normalized [Haar measure](../../../measure-theory.md#haar-measure):

$$
P_n\xi=\int_{\mathbb T}z^{-n}U_z\xi\,dz.
$$

Haar invariance gives $U_wP_n=w^nP_n$. Changing $z$ to $z^{-1}$ in the adjoint integral proves $P_n^*=P_n$. Applying the defining integral to $P_m\xi$ gives $P_nP_m=\delta_{nm}P_m$ by [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the characters $z^k$. Thus $P_n$ are [orthogonal projections](../../../hilbert-space.md#orthogonal-projection), and their ranges are exactly the indicated character subspaces.

It remains to prove completeness of these subspaces. The [Fejér kernel](../../../fourier-series.md#fejer-kernel) has the finite expansion

$$
K_N(e^{it})=\sum_{|n|<N}\left(1-\frac{|n|}{N}\right)e^{-int}
=\frac1N\left|\sum_{j=0}^{N-1}e^{ijt}\right|^2.
$$

It is nonnegative, has normalized integral one, and its integral outside any fixed neighborhood of the identity tends to zero, since the denominator in the usual geometric-sum formula is bounded away from zero there. Strong [continuity](../../../calculus.md#continuous-function) therefore gives

$$
\int K_N(z)U_z\xi\,dz\longrightarrow\xi:
$$

split the integral into that neighborhood, where $\|U_z\xi-\xi\|$ is small, and its complement, where it is bounded by $2\|\xi\|$. The integral on the left is $\sum_{|n|<N}(1-|n|/N)P_n\xi$. Hence the closed span of all $H_n$ is $H$. [Orthogonality](../../../linear-algebra.md#orthogonal-vectors) then gives the unweighted strong sum and the stated representation formula.

Conversely, any orthogonal decomposition indexed by the integers gives this representation; [continuity](../../../calculus.md#continuous-function) follows first on finite sums and then on all [vectors](../../../vector-space.md#vector) by the uniform unitary [norm](../../../functional-analysis.md#norm) bound. With $z=e^{it}$ its generator is

$$
A\xi=\sum_nnP_n\xi,\qquad
D(A)=\left\{\xi:\sum_nn^2\|P_n\xi\|^2<\infty\right\}.
$$

This diagonal operator is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) and $U_{e^{it}}=e^{itA}$. Thus the circle theorem is the integer-spectrum version of the one-parameter theorem.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Stone theorem for one-parameter unitary groups](../../../functional-analysis.md#stone-s-theorem-on-one-parameter-unitary-groups) states that every strongly continuous [unitary representation](../../../representation-theory.md#unitary-representation) $U_t$ of $\mathbb R$ is uniquely $U_t=e^{itA}$ for a possibly unbounded [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) $A$. Its domain is

$$
D(A)=\left\{\xi:\lim_{t\to0}\frac{U_t\xi-\xi}{it}\text{ exists in norm}\right\}.
$$

Conversely every [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) $A$ gives such a [group](../../../group.md) by the [Borel functional calculus for a normal operator](../../../banach-algebra.md#borel-functional-calculus-for-a-normal-operator).

Prove the forward direction by putting $G=iA$, initially defined as the [norm](../../../functional-analysis.md#norm) derivative at zero. Its domain is dense: for $f\in C_c^\infty(\mathbb R)$, the [vector](../../../vector-space.md#vector) $\xi_f=\int f(t)U_t\xi\,dt$ has derivative $G\xi_f=-\int f'(t)U_t\xi\,dt$. Smooth approximate identities make $\xi_f\to\xi$. The [group](../../../group.md) law gives $U_tD(G)=D(G)$ and $GU_t=U_tG$ on that domain. Differentiation of preserved [inner products](../../../linear-algebra.md#inner-product) shows that $G$ is skew-symmetric, so $A=-iG$ is symmetric.

The derivative operator is closed. Indeed, if $\xi_n\to\xi$ and $G\xi_n\to\eta$, integrate the orbit derivative to obtain

$$
U_t\xi_n-\xi_n=\int_0^tU_sG\xi_n\,ds.
$$

Taking limits gives the same identity with $\xi,\eta$; dividing by $t$ at zero proves $\xi\in D(G)$ and $G\xi=\eta$.

Now define bounded Laplace integrals

$$
R_+\xi=\int_0^\infty e^{-t}U_t\xi\,dt,\qquad
R_-\xi=\int_0^\infty e^{-t}U_{-t}\xi\,dt.
$$

Shifting the integration variable in $U_hR_\pm\xi$ and taking the derivative at zero shows that $R_\pm\xi\in D(G)$ and

$$
GR_+=R_+-I,\qquad GR_-=I-R_-.
$$

Hence $I-G$ and $I+G$ are both surjective. Since $G=iA$, this means $A+iI$ and $A-iI$ are surjective.

Here is why these range conditions establish self-adjointness rather than just symmetry. If $\eta\in D(A^*)$, solve $(A-iI)\xi=(A^*-iI)\eta$. Then $\eta-\xi\in\ker(A^*-iI)=\operatorname{Ran}(A+iI)^\perp=\{0\}$. Thus $D(A^*)\subseteq D(A)$, and symmetry gives equality with $A^*=A$.

The permitted functional calculus now gives $V_t=e^{itA}$. It is unitary, strongly continuous by dominated convergence against spectral measures, and differentiable with derivative $iAV_t\xi$ on $D(A)$. Differentiate $V_{-t}U_t\xi$ for $\xi\in D(A)$; the two derivative terms cancel because both [groups](../../../group.md) preserve the domain and commute with their generator. Its value is consequently the constant $\xi$. Density of the domain implies $U_t=V_t$ on all of $H$.

For completeness, the converse and the exact domain follow from the same calculus. If $\xi\in D(A)$, dominated convergence applied to $|(e^{it\lambda}-1)/t|\leq|\lambda|$ gives the derivative $iA\xi$. If that [norm](../../../functional-analysis.md#norm) derivative exists, Fatou's lemma applied to its squared [norm](../../../functional-analysis.md#norm) gives $\int\lambda^2\,d\langle E_A(\lambda)\xi,\xi\rangle<\infty$, so $\xi\in D(A)$. The derivative characterization also proves uniqueness. Thus

$$
\boxed{\text{strongly continuous unitary groups}\ \longleftrightarrow\ \text{self-adjoint generators}.}
$$

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a discrete [group](../../../group.md), one standard definition of amenability is the fixed-point property: every continuous affine action on a nonempty compact [convex set](../../../mathematical-optimization.md#convex-set) in a locally convex space has a fixed point. The equivalent state formulation, which may be stated without proof here, is that there is a left-invariant [invariant mean](../../../geometric-group-theory.md#invariant-mean) on $\ell^\infty(\Gamma)$. Equivalently, every [unital](../../../associative-algebra.md#unital-algebra) left-translation-invariant [star-subalgebra](../../../associative-algebra.md#star-subalgebra) of $\ell^\infty(\Gamma)$ admits a left-invariant state, with [continuity](../../../calculus.md#continuous-function) for the supremum [norm](../../../functional-analysis.md#norm); one may equally pass to its [norm](../../../functional-analysis.md#norm) [closure](../../../topology.md#closure-topology). A state means a positive [linear functional](../../../linear-algebra.md#linear-functional) of [norm](../../../functional-analysis.md#norm) one with value one on the constant function one. Restriction proves the [subalgebra](../../../algebra.md#subalgebra) formulation from the full-algebra version, and taking the full algebra proves the converse. Such a mean is finitely additive on [indicator functions](../../../measure-theory.md#indicator-function), not necessarily countably additive.

Write $(\lambda(g)\mu)(h)=\mu(g^{-1}h)$ on $\ell^1(\Gamma)$ and $(L_gf)(h)=f(g^{-1}h)$ on bounded functions. We prove equivalence of this mean condition, the [Reiter condition](../../../geometric-group-theory.md#reiter-condition), and existence of a [Følner sequence](../../../geometric-group-theory.md#folner-sequence).

Assume first that an [invariant mean](../../../geometric-group-theory.md#invariant-mean) $m$ exists. Fix a finite set $K\subseteq\Gamma$. In the real [Banach space](../../../banach-space.md) $\bigoplus_{g\in K}\ell^1(\Gamma)$ with sum [norm](../../../functional-analysis.md#norm), consider the [convex set](../../../mathematical-optimization.md#convex-set)

$$
\mathcal C=\{(\lambda(g)\mu-\mu)_{g\in K}:\mu\text{ a finitely supported probability measure}\}.
$$

If zero were outside its [norm](../../../functional-analysis.md#norm) [closure](../../../topology.md#closure-topology), the [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) would give bounded real functions $f_g$ and $\delta>0$ such that

$$
\sum_{g\in K}\sum_h f_g(h)[(\lambda(g)\mu)(h)-\mu(h)]\geq\delta
$$

for every such $\mu$. Testing point masses at $h$ shows

$$
\sum_{g\in K}[f_g(gh)-f_g(h)]\geq\delta\quad\text{for every }h.
$$

Applying the positive [invariant mean](../../../geometric-group-theory.md#invariant-mean) makes the left side zero and the right side at least $\delta$, a contradiction. Therefore zero is in the [closure](../../../topology.md#closure-topology): for any $\varepsilon>0$ a finitely supported [probability measure](../../../probability-theory.md#probability-measure) makes the sum of the translation defects over $K$ less than $\varepsilon$. Enumerate the countable [group](../../../group.md), take the first $n$ elements for $K$ and $\varepsilon=1/n$, and obtain a sequence satisfying the [Reiter condition](../../../geometric-group-theory.md#reiter-condition). This proves (1) implies (2).

Next assume (2). An $\ell^1$ [probability measure](../../../probability-theory.md#probability-measure) can be approximated in [norm](../../../functional-analysis.md#norm) by finitely supported [probability measures](../../../probability-theory.md#probability-measure), by restricting to a large finite set and renormalizing. Replacing $\mu$ by $\nu$ changes each defect by at most $2\|\mu-\nu\|_1$. Thus simultaneous small defects for finitely many translations can be achieved with finite support.

For such $\nu$, set $F_t=\{h:\nu(h)>t\}$. The elementary identity $|r-s|=\int_0^\infty|1_{r>t}-1_{s>t}|\,dt$ for $r,s\geq0$ gives

$$
\int_0^\infty|F_t|\,dt=1,\qquad
\int_0^\infty|F_t\mathbin\triangle gF_t|\,dt
=\|\lambda(g)\nu-\nu\|_1.
$$

If the sum of defects over $K$ is less than $\varepsilon$, some $t$ with $F_t\ne\varnothing$ must satisfy $\sum_{g\in K}|F_t\triangle gF_t|<\varepsilon|F_t|$; otherwise integration would contradict that strict inequality. Applying this [layer-cake extraction of Følner sets](../../../geometric-group-theory.md#layer-cake-extraction-of-folner-sets) to successive finite sets of translations gives nonempty finite $F_n$ with each relative boundary tending to zero. Hence (2) implies (3).

Conversely, normalized counting measures $\mu_n=1_{F_n}/|F_n|$ satisfy

$$
\|\lambda(g)\mu_n-\mu_n\|_1=\frac{|gF_n\triangle F_n|}{|F_n|},
$$

so (3) implies (2). Finally, from (2) define states $m_n(f)=\sum_h\mu_n(h)f(h)$. The dual [unit ball](../../../functional-analysis.md#unit-ball) of $\ell^\infty(\Gamma)$ is weak-star compact by the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem); take a convergent subnet, since this [compactness](../../../topology.md#compact-space) need not be metrizable. Its limit $m$ is positive with $m(1)=1$, and

$$
|m_n(L_gf)-m_n(f)|\leq\|f\|_\infty\|\lambda(g^{-1})\mu_n-\mu_n\|_1\longrightarrow0.
$$

Thus $m$ is invariant, proving (2) implies (1). Together these implications establish all three equivalences. Countability is used to obtain sequences from finite tests; it is not a justification for replacing the [compactness](../../../topology.md#compact-space) subnet by a subsequence.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Assume the invariant set $C$ is nonempty, as required for any fixed-point assertion. For $x\in C$, put $r(x)=\sup_{c\in C}\|x-c\|$ and $r_*=\inf_{x\in C}r(x)$. Boundedness makes these finite. The parallelogram identity gives, for $x,y\in C$,

$$
r\left(\frac{x+y}{2}\right)^2
\leq\frac{r(x)^2+r(y)^2}{2}-\frac{\|x-y\|^2}{4}.
$$

The midpoint lies in $C$, so a minimizing sequence $x_n$ satisfies

$$
\|x_n-x_m\|^2\leq2r(x_n)^2+2r(x_m)^2-4r_*^2\longrightarrow0.
$$

Since $C$ is closed in a [Hilbert space](../../../hilbert-space.md), the sequence converges to $x_*\in C$. The function $r$ is 1-Lipschitz, hence $r(x_*)=r_*$. The same midpoint inequality proves uniqueness of this minimizing center.

An affine isometry from the [group](../../../group.md) maps $C$ onto itself, since its inverse also preserves $C$. Therefore it preserves $r$ and sends its unique minimizer to another minimizer. Uniqueness gives

$$
\boxed{gx_*=x_*\quad\text{for every group element }g.}
$$

This proof applies to a closed bounded convex subset, the substantive meaning of the printed “convex subspace”; if it is literally a bounded [vector](../../../vector-space.md#vector) subspace, it is just the zero subspace.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The topology needed here is the [weak-star topology](../../../weak-topology.md#weak-star-topology) $\sigma(E^*,E)$, meaning pointwise convergence on $E$. With the literal [weak topology](../../../weak-topology.md) $\sigma(E^*,E^{**})$, the claimed [compactness](../../../topology.md#compact-space) is false. For example, $E=c_0$ is separable and $E^*=\ell^1$. Its unit [vectors](../../../vector-space.md#vector) $e_n$ have no weak cluster point: every coordinate functional forces a cluster point to have all coordinates zero, while the bounded functional $x\mapsto\sum_jx_j$ has value one throughout. Thus the dual [unit ball](../../../functional-analysis.md#unit-ball) is not [weakly compact](../../../weak-topology.md#weakly-compact-set). We prove the intended weak-star assertion in full.

Choose a countable dense set $(x_k)$ in the [unit ball](../../../functional-analysis.md#unit-ball) of $E$. On $E_1^*$ define

$$
\boxed{d(\phi,\psi)=\sum_{k\geq1}2^{-k}|\phi(x_k)-\psi(x_k)|.}
$$

Each term is at most $2\cdot2^{-k}$, so the series converges. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) is immediate, and $d=0$ forces equality on the dense set and hence on all of $E$. It is therefore a metric. Convergence in this metric is equivalent to convergence on every $x_k$: one direction follows from any individual term, and the other by bounding the series tail uniformly. Because $\|\phi\|,\|\psi\|\leq1$, approximation of any unit [vector](../../../vector-space.md#vector) by $x_k$ then gives convergence on all of $E$. The same finite-tail and approximation argument for neighborhoods proves equality with the [weak-star topology](../../../weak-topology.md#weak-star-topology), not just agreement of its convergent sequences.

Given a sequence $(\phi_n)$ in this ball, diagonal selection gives a subsequence converging at every $x_k$, since each coordinate lies in a compact disk. Uniform [norm](../../../functional-analysis.md#norm) bounds then make it pointwise Cauchy at every $x\in E$. Define $\phi(x)$ as the limit. [Linearity](../../../vector-space.md#linearity) passes to the limit, and $|\phi(x)|\leq\|x\|$, so $\phi\in E_1^*$. The subsequence converges to it in the metric. Thus this [metric space](../../../topological-analysis.md#metric-space) is sequentially compact, hence compact, proving

$$
\boxed{E_1^*\text{ is compact and metrizable in }\sigma(E^*,E).}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use the same intended [weak-star topology](../../../weak-topology.md#weak-star-topology) as in (b), and assume $C\ne\varnothing$. The induced operator is $T=S^*$, so $T\phi(x)=\phi(Sx)$; it is weak-star continuous because evaluation after applying $T$ is still evaluation at a [vector](../../../vector-space.md#vector) of $E$.

Choose $\phi\in C$ and form the averages

$$
\phi_n=\frac1n\sum_{j=0}^{n-1}T^j\phi.
$$

Invariance and convexity put every $\phi_n$ in $C$. Weak-star closedness and (b) make $C$ compact, so some subsequence converges to $\psi\in C$. Telescoping gives

$$
T\phi_n-\phi_n=\frac{T^n\phi-\phi}{n},\qquad
\|T\phi_n-\phi_n\|\leq\frac2n,
$$

because both orbit points lie in the dual [unit ball](../../../functional-analysis.md#unit-ball). Weak-star [continuity](../../../calculus.md#continuous-function) now gives $T\psi-\psi=0$. Hence $\boxed{T\text{ has a fixed point in }C.}$ This is the [weak-star fixed point theorem for an adjoint operator](../../../weak-topology.md#weak-star-fixed-point-theorem-for-an-adjoint-operator); it does not require $T$ to be a contraction on the entire [dual space](../../../linear-algebra.md#dual-space).

If “weakly closed” is interpreted literally as closed for $\sigma(E^*,E^{**})$, the result can fail. Take $E=c_0$, let $S$ be the left shift and $T=S^*$ the right shift on $\ell^1$. The set

$$
C=\{x\in\ell^1:x_j\geq0,\ \sum_jx_j=1\}
$$

is a nonempty weakly closed convex subset of the [unit ball](../../../functional-analysis.md#unit-ball): its defining coordinate inequalities and sum equality are weakly closed. It is invariant under the right shift. But a fixed [vector](../../../vector-space.md#vector) of that shift has first coordinate zero and then every coordinate zero, so none belongs to $C$. This supplies a counterexample to the literal topology and explains why the weak-star qualification is essential.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Put $F=\ker(I-U)$. For a [unitary operator](../../../vector-space.md#unitary-operator), $\ker(I-U^*)=F$, so

$$
H=F\oplus\overline{\operatorname{Ran}(I-U)}.
$$

This follows from the general identity $\operatorname{Ran}(A)^\perp=\ker A^*$. The averaging operators have $\|T_n\|\leq1$ and equal the identity on $F$. On a [vector](../../../vector-space.md#vector) $(I-U)\eta$, telescoping gives

$$
T_n(I-U)\eta=\frac{I-U^n}{n}\eta,\qquad
\|T_n(I-U)\eta\|\leq\frac{2\|\eta\|}{n}\longrightarrow0.
$$

The uniform [norm](../../../functional-analysis.md#norm) bound extends this convergence to the [closure](../../../topology.md#closure-topology) of the range. Thus $T_n$ tends to identity on $F$ and to zero on its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). Consequently

$$
\boxed{T_n\xi\longrightarrow P\xi\quad\text{for every }\xi\in H,}
$$

which is exactly convergence in the [strong operator topology](../../../functional-analysis.md#strong-operator-topology). This proves the [Von Neumann mean ergodic theorem](../../../vector-space.md#von-neumann-mean-ergodic-theorem) in the requested unitary case.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For a [unital](../../../associative-algebra.md#unital-algebra) [star-subalgebra](../../../associative-algebra.md#star-subalgebra) $A\subseteq B(H)$, the [Von Neumann double commutant theorem](../../../associative-algebra.md#von-neumann-double-commutant-theorem) states

$$
\boxed{\overline A^{\mathrm{SOT}}=\overline A^{\mathrm{WOT}}=A''.}
$$

Here $A'$ is the [commutant of an operator algebra](../../../associative-algebra.md#commutant-of-an-operator-algebra), consisting of operators commuting with every element of $A$. The double commutant is closed in either topology: multiplication by a fixed [bounded operator](../../../topological-vector-space.md#continuous-linear-operator) is continuous in both. Therefore both closures of $A$ lie in $A''$.

For the converse, let $T\in A''$ and choose finitely many [vectors](../../../vector-space.md#vector) $\xi_1,\ldots,\xi_n$. In $H^n$ put

$$
K=\overline{\{(a\xi_1,\ldots,a\xi_n):a\in A\}}.
$$

It is invariant under the diagonal action of $A$ and its adjoints, so its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $Q$ commutes with that diagonal action. Consequently each [matrix](../../../vector-space.md#matrix) entry $Q_{ij}$ belongs to $A'$. The diagonal operator with entry $T$ therefore commutes with $Q$. Since $I\in A$, the tuple $\xi=(\xi_1,\ldots,\xi_n)$ belongs to $K$, and hence so does $(T\xi_1,\ldots,T\xi_n)$. By the definition of $K$, one element $a\in A$ approximates this entire tuple arbitrarily closely. This is exactly approximation in every strong-operator neighborhood of $T$. It proves $A''\subseteq\overline A^{\mathrm{SOT}}$ and thus both asserted equalities. In particular, $M=A''$ is a [Von Neumann algebra](../../../functional-analysis.md#von-neumann-algebra).

The [Kaplansky density theorem](../../../associative-algebra.md#kaplansky-density-theorem) strengthens the result by preserving [norm](../../../functional-analysis.md#norm) bounds:

$$
\boxed{\overline{\{a\in A:\|a\|\leq1\}}^{\mathrm{SOT}}
=\{x\in M:\|x\|\leq1\}.}
$$

It also holds for the [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) and positive unit balls; the full ball can in fact be approximated in the [strong-star topology](../../../functional-analysis.md#strong-star-operator-topology), meaning strong convergence of both operators and adjoints. We prove the bound rather than merely scaling the unbounded approximants furnished by the double commutant theorem.

First put $C=\overline A^{\|\cdot\|}$, a [unital](../../../associative-algebra.md#unital-algebra) [C-star algebra](../../../banach-algebra.md#c-star-algebra). Its [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) part is weak-operator dense in $M_{\mathrm{sa}}$: symmetrize any weak approximating net. For a convex subset, strong and weak operator closures agree. To see this explicitly, separation from a strong [closure](../../../topology.md#closure-topology) supplies a continuous real functional on finitely many image [vectors](../../../vector-space.md#vector), hence one of the form $\operatorname{Re}\sum_j\langle a\xi_j,\eta_j\rangle$, which is also weak-operator continuous. The [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) would then separate the point from the weak [closure](../../../topology.md#closure-topology) as well. Thus every [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) $x\in M$ is a strong limit of [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) $a_i\in C$, initially without a common [norm](../../../functional-analysis.md#norm) bound.

The needed functional-calculus [continuity](../../../calculus.md#continuous-function) follows directly from [resolvents](../../../functional-analysis.md#resolvent-of-an-operator). The [resolvent identity](../../../banach-algebra.md#resolvent-identity) gives

$$
(a_i-iI)^{-1}-(x-iI)^{-1}
=(a_i-iI)^{-1}(x-a_i)(x-iI)^{-1}.
$$

The first factor has [norm](../../../functional-analysis.md#norm) at most one, so the right side tends strongly to zero. The same holds at $-i$. Both [resolvent](../../../functional-analysis.md#resolvent-of-an-operator) nets are uniformly bounded, so their products converge strongly. Their scalar functions generate a [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) algebra separating points of $\mathbb R$ and vanishing at infinity. The [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem), applied to the one-point compactification, makes this algebra uniformly dense in $C_0(\mathbb R)$. Uniform approximation and the functional-calculus [norm](../../../functional-analysis.md#norm) bound therefore show

$$
f(a_i)\longrightarrow f(x)\text{ strongly for every }f\in C_0(\mathbb R).
$$

This proves [strong continuity of functional calculus through resolvents](../../../banach-algebra.md#strong-continuity-of-functional-calculus-through-resolvents) without an unjustified uniform bound on the original $a_i$.

If $x=x^*$ and $\|x\|\leq1$, choose a real compactly supported continuous $f$ equal to the identity on $[-1,1]$ and bounded in absolute value by one. Then $f(a_i)\in C$ are [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) contractions and converge strongly to $f(x)=x$. For a positive contraction $x$, choose instead $0\leq f\leq1$ equal to the identity on $[0,1]$; this gives positive contractions. These prove the two restricted versions for $C$.

For an arbitrary contraction $x\in M$, apply the [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) result in the [matrix algebra](../../../associative-algebra.md#matrix-algebra) $M_2(C)$ to

$$
X=\begin{pmatrix}0&x\\x^*&0\end{pmatrix},\qquad \|X\|=\|x\|\leq1.
$$

The strong [closure](../../../topology.md#closure-topology) of $M_2(C)$ is $M_2(M)$, since finitely many entries may be approximated simultaneously. The upper-right entries $c_i$ of the approximating [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) contraction [matrices](../../../vector-space.md#matrix) belong to $C$, satisfy $\|c_i\|\leq1$, and converge strongly to $x$. The lower-left entries are $c_i^*$ and converge strongly to $x^*$. This proves the full strong-star assertion for $C$.

Finally transfer the bounds from $C$ to the possibly nonclosed algebra $A$. A contraction $c\in C$ has an approximant $b\in A$ with $\|b-c\|<\varepsilon$, so $b/(1+\varepsilon)$ is an $A$-contraction within $2\varepsilon$ of $c$. [Self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) approximants are obtained by symmetrizing first. For a positive contraction, approximate $c^{1/2}$ by $b\in A$ and use the positive contraction $b^*b/(1+\varepsilon)^2$, which tends in [norm](../../../functional-analysis.md#norm) to $c$ as $\varepsilon\downarrow0$. Combining these [norm](../../../functional-analysis.md#norm) approximations with each finite-vector strong approximation proves all versions for $A$. The reverse inclusions follow because the relevant [norm](../../../functional-analysis.md#norm) bounds and the inequalities defining a [positive operator](../../../hilbert-space.md#positive-operator) are preserved by strong limits.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Interpret the involution as the adjoint for the Hilbert-space structure on $V$. The hypotheses make $\Omega$ a [cyclic vector for an operator algebra](../../../functional-analysis.md#cyclic-vector-for-an-operator-algebra) for both $A$ and $A'$. They also make it a [separating vector](../../../functional-analysis.md#separating-vector-for-an-operator-algebra) for each: if $a\Omega=0$, then $a$ vanishes on $A'\Omega=V$, and similarly for $A'$. Thus the [Tomita operator](../../../functional-analysis.md#tomita-operator)

$$
S(a\Omega)=a^*\Omega
$$

is well defined, antilinear, invertible and satisfies $S^2=I$. Define the [modular operator](../../../functional-analysis.md#modular-operator) and [modular conjugation](../../../functional-analysis.md#modular-conjugation) by

$$
\boxed{\Delta=S^*S,\qquad J=S\Delta^{-1/2},\qquad S=J\Delta^{1/2}.}
$$

We calculate them explicitly to prove the commutant assertion.

The finite-dimensional structure of a [unital](../../../associative-algebra.md#unital-algebra) [star-algebra](../../../associative-algebra.md#star-algebra) gives an orthogonal decomposition

$$
V=\bigoplus_j(\mathbb C^{n_j}\otimes\mathbb C^{m_j}),\qquad
A=\bigoplus_j(M_{n_j}(\mathbb C)\otimes I_{m_j}),\qquad
A'=\bigoplus_j(I_{n_j}\otimes M_{m_j}(\mathbb C)).
$$

This is the usual matrix-block structure: minimal central [projections](../../../vector-space.md#projection-linear-algebra) separate the simple summands, and each simple [matrix algebra](../../../associative-algebra.md#matrix-algebra) acts as its defining representation with a multiplicity space. Identify each [vector](../../../vector-space.md#vector) block with an $n_j$-by-$m_j$ [matrix](../../../vector-space.md#matrix) $D_j$ with its [Hilbert-Schmidt](../../../compact-operator.md#hilbert-schmidt-operator) [inner product](../../../linear-algebra.md#inner-product). The two algebras act by left and right multiplication. If $D_j$ has rank $r_j$, the left orbit has dimension $n_jr_j$ and the right orbit dimension $m_jr_j$. Cyclicity on both sides therefore forces $r_j=m_j=n_j$. Every $D_j$ is square and invertible.

Right multiplication by a suitable unitary is a unitary change of this identification commuting with the left algebra. The polar decomposition of each $D_j$ therefore lets us assume $D_j>0$. In one such block, for an arbitrary [matrix](../../../vector-space.md#matrix) $X=aD$, the [Tomita operator](../../../functional-analysis.md#tomita-operator) is

$$
S(X)=D^{-1}X^*D.
$$

Its polar factors are

$$
\boxed{J(X)=X^*,\qquad \Delta^{1/2}(X)=DXD^{-1},\qquad
\Delta(X)=D^2XD^{-2}.}
$$

Indeed, $J$ is an antiunitary involution and $J\Delta^{1/2}(X)=D^{-1}X^*D$. The fact that $\Delta^{1/2}$ is a [positive operator](../../../hilbert-space.md#positive-operator) is transparent in a [basis](../../../vector-space.md#basis) diagonalizing $D$: it multiplies the [matrix](../../../vector-space.md#matrix) unit $E_{kl}$ by the positive ratio $d_k/d_l$. These are therefore the unique polar factors of $S$.

Finally, if $L_a$ denotes left multiplication,

$$
(JL_aJ)(X)=(aX^*)^*=Xa^*.
$$

As $a$ ranges over the full [matrix](../../../vector-space.md#matrix) block, these are exactly its right multiplications. Applying this on every block and transporting back by the unitary identifications proves

$$
\boxed{JAJ=A'.}
$$

This also establishes the required modular definitions intrinsically, independent of the chosen [matrix](../../../vector-space.md#matrix) coordinates.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Write $M=\lambda(\Gamma)''$, the [group von Neumann algebra](../../../functional-analysis.md#group-von-neumann-algebra), and define right translations by $\rho(g)\delta_h=\delta_{hg^{-1}}$. Left and right translations commute, so every $T\in M$ commutes with every $\rho(g)$. A [Von Neumann factor](../../../functional-analysis.md#von-neumann-factor) means that the center of $M$ is exactly $\mathbb CI$.

Suppose every nonidentity [conjugacy class](../../../group-theory.md#conjugacy-class) is infinite and $T$ is central. Put $\eta=T\delta_e$. Since $T$ commutes with both regular actions and $\lambda(g)\rho(g)\delta_e=\delta_e$,

$$
\lambda(g)\rho(g)\eta=\eta.
$$

The action on a [basis](../../../vector-space.md#basis) [vector](../../../vector-space.md#vector) is $\delta_h\mapsto\delta_{ghg^{-1}}$, so the coefficients of $\eta\in\ell^2(\Gamma)$ are constant on conjugacy classes. A nonzero constant on an infinite class would have infinite squared sum. Thus all coefficients away from the identity vanish and $\eta=c\delta_e$.

Commutation with the right action now gives $T\delta_h=c\delta_h$ for every $h$, because those [vectors](../../../vector-space.md#vector) form the right orbit of $\delta_e$. Hence $T=cI$ and $M$ is a factor. This argument also shows that $\delta_e$ is separating for $M$.

Conversely, if a nonidentity class $C$ is finite, then

$$
Z=\sum_{h\in C}\lambda(h)\in M
$$

commutes with every $\lambda(g)$, since conjugation permutes $C$. Therefore $Z\in M\cap\lambda(\Gamma)'=Z(M)$. It is not scalar: $Z\delta_e=\sum_{h\in C}\delta_h$ is nonzero and orthogonal to $\delta_e$. Consequently $M$ is not a factor. We have proved

$$
\boxed{\lambda(\Gamma)''\text{ is a factor}\iff\Gamma\text{ is an ICC group}.}
$$

The condition is vacuous for the trivial [group](../../../group.md), whose algebra $\mathbb CI$ is indeed a factor.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

The dense commutant orbit makes $\Omega$ separating for $M$, so $S_0(a\Omega)=a^*\Omega$ is well defined on the dense subspace $M\Omega$. Put $\tau(a)=\langle a\Omega,\Omega\rangle$. The assumed identity says that this positive [vector](../../../vector-space.md#vector) functional is a [tracial positive functional](../../../banach-algebra.md#tracial-positive-functional). Hence

$$
\|S_0(a\Omega)\|^2=\tau(aa^*)=\tau(a^*a)=\|a\Omega\|^2.
$$

It extends to an antiunitary involution $J$ on $H$, with $J\Omega=\Omega$. This is the [modular conjugation](../../../functional-analysis.md#modular-conjugation), and the [modular operator](../../../functional-analysis.md#modular-operator) in this tracial case is $\Delta=I$.

On the dense subspace $M\Omega$,

$$
(JaJ)(b\Omega)=J(ab^*\Omega)=ba^*\Omega.
$$

Thus it acts by right multiplication and commutes with all left multiplications; $JMJ\subseteq M'$. We prove the reverse inclusion rather than assuming the general Tomita commutation theorem.

Let $T\in M'$, $C=\|T\|$, and $\eta=T\Omega$. The set

$$
\mathcal B=\{a\Omega:a\in M,\ \|a\|\leq C\}
$$

is [weakly compact](../../../weak-topology.md#weakly-compact-set) and convex. Indeed, [trace-class duality](../../../compact-operator.md#trace-class-duality) and the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) make the bounded-operator ball compact in a topology stronger than the [weak operator topology](../../../functional-analysis.md#weak-operator-topology). The algebra $M$ is weak-operator closed, and $a\mapsto a\Omega$ is weakly continuous, so its image is [weakly compact](../../../weak-topology.md#weakly-compact-set).

For $b\in M$ use the [polar decomposition of a bounded operator](../../../banach-algebra.md#polar-decomposition-of-a-bounded-operator) $b=uh$, $h=|b|$. Both $h$ and $u$ belong to $M$: [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) gives $h$, and $b(h+\varepsilon I)^{-1}$ tends strongly to $u$. The polar decomposition is proved independently in Question 8. Since $T$ commutes with $M$,

$$
\langle T\Omega,b\Omega\rangle
=\langle T h^{1/2}u^*\Omega,h^{1/2}\Omega\rangle.
$$

The [trace](../../../linear-algebra.md#matrix-trace) identity gives

$$
\|h^{1/2}u^*\Omega\|^2=\tau(uhu^*)=\tau(hu^*u)=\tau(h),
\qquad \|h^{1/2}\Omega\|^2=\tau(h).
$$

Therefore $|\langle\eta,b\Omega\rangle|\leq C\tau(h)$. Meanwhile

$$
\sup_{a\in M,\ \|a\|\leq C}\operatorname{Re}\langle a\Omega,b\Omega\rangle
=C\tau(h),
$$

with the supremum attained by $a=Cu$. For the upper bound, traciality gives $\tau(b^*a)=\tau(h^{1/2}u^*a h^{1/2})$; evaluating this on $\Omega$ bounds its absolute value by $\|a\|\tau(h)$.

These support inequalities imply $\eta\in\mathcal B$. Otherwise the [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) would separate $\eta$ from this closed [convex set](../../../mathematical-optimization.md#convex-set) by a real inner-product functional. Since $M\Omega$ is dense, its separating [vector](../../../vector-space.md#vector) could be approximated by some $b\Omega$, preserving strict separation, contrary to the displayed inequality. Thus $T\Omega=a\Omega$ for an $a\in M$ of [norm](../../../functional-analysis.md#norm) at most $C$.

The [bounded operator](../../../topological-vector-space.md#continuous-linear-operator) $R_a=Ja^*J$ commutes with $M$ and sends $\Omega$ to $a\Omega$. It agrees with $T$ on the cyclic [vector](../../../vector-space.md#vector) and therefore on all of $M\Omega$, hence on $H$. This proves $T\in JMJ$, and so

$$
\boxed{JMJ=M'.}
$$

For the regular representation, take $\Omega=\delta_e$. It is cyclic for the left action and for the commuting right action. On finite sums of left translations, its [vector](../../../vector-space.md#vector) functional is the identity coefficient, so $\tau(ab)=\tau(ba)$. This extends to the whole [group von Neumann algebra](../../../functional-analysis.md#group-von-neumann-algebra) by the bounded strong-star approximations of Question 6, taking limits of the [vector](../../../vector-space.md#vector) functional and products. The conjugation is explicitly

$$
(J\xi)(h)=\overline{\xi(h^{-1})},\qquad J\lambda(g)J=\rho(g).
$$

Consequently

$$
\boxed{\lambda(\Gamma)'=J\lambda(\Gamma)''J=\rho(\Gamma)''.}
$$

Thus the commutant in (b) is exactly the [Von Neumann algebra](../../../functional-analysis.md#von-neumann-algebra) of right regular translations, with the inverse in $\rho(g)$ fixing the representation convention.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

A bounded [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) $T$ is a [positive operator](../../../hilbert-space.md#positive-operator) when $\langle T\xi,\xi\rangle\geq0$ for every $\xi$. Equivalently its [quadratic form](../../../linear-algebra.md#quadratic-form) is nonnegative. We construct its [positive square root of an operator](../../../hilbert-space.md#positive-square-root-of-an-operator) directly and prove uniqueness.

If $T=0$ its positive square root is zero. Otherwise set $r=\|T\|$, $B=T/r$, and $C=I-B$. Then $0\leq B\leq I$ and $C$ is positive. It is also a contraction. Indeed, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for the positive form $\langle B\xi,\eta\rangle$ gives $\|B\xi\|^2\leq\langle B\xi,\xi\rangle$, and hence

$$
\|C\xi\|^2=\|\xi\|^2-2\langle B\xi,\xi\rangle+\|B\xi\|^2\leq\|\xi\|^2.
$$

The scalar binomial series has the form

$$
\sqrt{1-z}=1-\sum_{n\geq1}c_nz^n,\qquad
c_n=\frac{\binom{2n}{n}}{4^n(2n-1)}>0,\qquad\sum_{n\geq1}c_n=1.
$$

The last equality follows by taking $z\uparrow1$ in the nonnegative series. Therefore

$$
S=\sqrt r\left(I-\sum_{n\geq1}c_nC^n\right)
$$

converges in [operator norm](../../../continuous-dual-space.md#operator-norm). Every $C^n$ is a positive contraction: its even powers are squares, its odd powers have form $C^kCC^k$, and their [norms](../../../functional-analysis.md#norm) are at most one. Each partial sum for $S/\sqrt r$ is consequently positive, since it is at least $(1-\sum_{n\leq N}c_n)I$. The limit is positive. Multiplying the absolutely convergent series and using the scalar coefficient identity gives $S^2=r(I-C)=T$. This construction also shows that $S$ is a [norm](../../../functional-analysis.md#norm) limit of polynomials in $T$ and thus commutes with every operator commuting with $T$.

Now suppose $R$ is another positive square root. It commutes with $T=R^2$, hence with $S$. Thus

$$
(R-S)(R+S)=R^2-S^2=0.
$$

The difference vanishes on the range of $R+S$ and on its [closure](../../../topology.md#closure-topology). It also vanishes on its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map): if $(R+S)\xi=0$, the fact that $R$ and $S$ are [positive operators](../../../hilbert-space.md#positive-operator) gives $\langle R\xi,\xi\rangle=\langle S\xi,\xi\rangle=0$, and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for their positive forms implies $R\xi=S\xi=0$. Since $R+S$ is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator), the orthogonal sum of its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and closed range is all of $H$. Therefore $R=S$, proving

$$
\boxed{T\geq0\Longrightarrow\text{a unique }T^{1/2}\geq0\text{ with }(T^{1/2})^2=T.}
$$

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

The [polar decomposition of a bounded operator](../../../banach-algebra.md#polar-decomposition-of-a-bounded-operator) states that every bounded $T:H\to H$ is uniquely

$$
\boxed{T=V|T|,\qquad |T|=(T^*T)^{1/2},\qquad \ker V=\ker T,}
$$

where $V$ is a [partial isometry](../../../banach-algebra.md#partial-isometry) with initial space $\overline{\operatorname{Ran}|T|}=(\ker T)^\perp$ and final space $\overline{\operatorname{Ran}T}$. Its initial and final [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) are $V^*V$ and $VV^*$.

Existence of $|T|$ was proved in (a). For every $\xi$,

$$
\||T|\xi\|^2=\langle T^*T\xi,\xi\rangle=\|T\xi\|^2.
$$

Thus the map $|T|\xi\mapsto T\xi$ is well defined and isometric on $\operatorname{Ran}|T|$. It extends uniquely to an isometry between its closed range and $\overline{\operatorname{Ran}T}$. Extend it by zero on $\ker|T|=\ker T$ to obtain $V$. The equation and the [projection](../../../vector-space.md#projection-linear-algebra) assertions follow immediately. Any other normalized [partial isometry](../../../banach-algebra.md#partial-isometry) with the same product must agree on the dense range of $|T|$ and vanish on its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement), giving uniqueness. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) normalization is essential; without it an action on the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) could be added.

A useful consequence for a [Von Neumann algebra](../../../functional-analysis.md#von-neumann-algebra) $M$ is that the polar factors of $T\in M$ also belong to $M$. The polynomial construction in (a) puts $|T|$ in the norm-closed algebra $M$. For $\varepsilon>0$, the inverse of $|T|+\varepsilon I$ belongs to $M$ by a convergent Neumann series, and

$$
T(|T|+\varepsilon I)^{-1}\longrightarrow V\quad\text{strongly}.
$$

These operators are contractions, since $\||T|\xi\|\leq\|(|T|+\varepsilon I)\xi\|$. On [vectors](../../../vector-space.md#vector) $|T|\xi$ the difference from $V$ has [norm](../../../functional-analysis.md#norm) at most $\varepsilon\|\xi\|$, and on the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) it is zero. Density and the uniform bound prove the strong limit. Strong closedness of $M$ then gives $V\in M$. This justifies the use of algebra-valued polar factors in Question 7(c).

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

A closed subspace invariant under a [star-algebra](../../../associative-algebra.md#star-algebra) is reducing, since it is invariant under every adjoint as well. Thus the [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) $P_1,P_2$ onto $H_1,H_2$ commute with $M$. Consider the bounded intertwiner

$$
T=(I-P_2)|_{H_1}:H_1\longrightarrow H_2^\perp.
$$

Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $H_1\cap H_2$, so its initial polar space is

$$
K_1=H_1\cap(H_1\cap H_2)^\perp.
$$

Its closed range is

$$
K_2=\overline{H_1+H_2}\cap H_2^\perp.
$$

For the inclusion from left to right, $(I-P_2)h_1=h_1-P_2h_1$ lies in $H_1+H_2$ and is orthogonal to $H_2$. Conversely, approximate any $z$ in the displayed $K_2$ by $h_{1,n}+h_{2,n}$ and apply $I-P_2$. The images converge to $z$ and equal $Th_{1,n}$, proving the reverse inclusion after [closure](../../../topology.md#closure-topology). The overline on the sum is present in the original PDF and is essential for potentially nonclosed sums.

Take the polar decomposition $T=V|T|$ between these [Hilbert spaces](../../../hilbert-space.md). Because $T$ intertwines the two actions of $M$, its adjoint does also, so $T^*T$ commutes with the action on $H_1$. Its positive square root therefore commutes as well. The identity $V|T|\xi=T\xi$ shows on its dense initial range that $V$ intertwines, and [continuity](../../../calculus.md#continuous-function) extends this to $K_1$. It is an isometry onto $K_2$. Consequently

$$
\boxed{H_1\cap(H_1\cap H_2)^\perp
\ \cong_M\ \overline{H_1+H_2}\cap H_2^\perp.}
$$

The unitary here is a unitary between the indicated [Hilbert space modules](../../../functional-analysis.md#hilbert-space-module-over-a-von-neumann-algebra), not an assertion that the unclosed algebraic sum is a [Hilbert space](../../../hilbert-space.md).

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

One implication is immediate: a unitary module equivalence makes each space an isometric copy of the entire other space, which is closed and invariant. For the converse, choose isometric intertwiners $u:H_1\to H_2$ and $v:H_2\to H_1$ supplied by the two embeddings. Their ranges are closed reducing subspaces. We construct the unitary, proving the [Schröder-Bernstein theorem for Hilbert space modules](../../../functional-analysis.md#schroder-bernstein-theorem-for-hilbert-space-modules) in this setting.

Put $w=vu$, an isometric intertwiner of $H_1$ into itself, and let $D=H_1\ominus vH_2$. The spaces $w^nD$, $n\geq0$, are mutually orthogonal. For $m>n$, applying the isometry relation reduces their [inner product](../../../linear-algebra.md#inner-product) to one between $D$ and $w^{m-n}D\subseteq wH_1\subseteq vH_2$, which is zero. Hence

$$
K=\bigoplus_{n\geq0}w^nD
$$

is a closed reducing submodule of $H_1$, and $K=D\oplus wK$. Its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) lies in $vH_2$, because it is orthogonal to $D$. Combining these decompositions gives

$$
vH_2=wK\oplus K^\perp.
$$

Apply the inverse isometry $v^*$ on $vH_2$ to obtain

$$
H_2=uK\oplus v^*K^\perp.
$$

The operator

$$
\boxed{W\xi=u\xi\quad(\xi\in K),\qquad
W\xi=v^*\xi\quad(\xi\in K^\perp)}
$$

is therefore an isometry onto $H_2$: it is isometric on each orthogonal summand and their images are the two orthogonal summands just exhibited. Both pieces intertwine the action of $M$, as do the [projections](../../../vector-space.md#projection-linear-algebra) onto $K$ and $K^\perp$, so $W$ is a unitary module equivalence. This proves the reverse implication with no finiteness assumption on either module.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
