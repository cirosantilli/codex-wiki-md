# Paper 111

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_111.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_111.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A sufficient absolute constant is $\boxed{C=16}$. The proof is a [density increment](../../../additive-combinatorics.md#density-increment) argument for a [cap set](../../../combinatorics.md#cap-set) over the [finite field](../../../algebra.md#finite-field) $\mathbb F_3$.

First work in $V=\mathbb F_3^d$, write $N=3^d$, and let $f=1_A$ be the [indicator function](../../../measure-theory.md#indicator-function) of a [cap set](../../../combinatorics.md#cap-set) of [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) $\alpha>0$. All [expectations](../../../probability-theory.md#expected-value) below are uniform. In [characteristic](../../../algebra.md#characteristic-of-a-field) three, a solution of $x+y+z=0$ having two equal entries has all three equal. Consequently the normalized [linear configuration count](../../../additive-combinatorics.md#linear-configuration-count) is

$$
T=\mathbb E_{x,y}f(x)f(y)f(-x-y)=\frac{|A|}{N^2}=\frac\alpha N.
$$

Set $\omega=e^{2\pi i/3}$ and use [Fourier analysis on a finite abelian group](../../../additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group) with

$$
\widehat f(\xi)=\mathbb E_x f(x)\omega^{-\xi\cdot x}.
$$

The [orthogonality of roots of unity](../../../algebra.md#orthogonality-of-roots-of-unity) and the [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) give

$$
T=\sum_{\xi\in V}\widehat f(\xi)^3,
\qquad
\widehat f(0)=\alpha,
\qquad
\sum_{\xi\ne0}|\widehat f(\xi)|^2=\alpha-\alpha^2.
$$

If $N\alpha^2\geq2$, then $\alpha<1$ for a [cap set](../../../combinatorics.md#cap-set) and

$$
\frac{\alpha^3}{2}
\leq\alpha^3-\frac\alpha N
\leq\sum_{\xi\ne0}|\widehat f(\xi)|^3
\leq\left(\max_{\xi\ne0}|\widehat f(\xi)|\right)(\alpha-\alpha^2).
$$

Thus some nonzero [finite abelian Fourier coefficient](../../../additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group) has magnitude at least $\alpha^2/2$.

For this $\xi$, let $\alpha_j$ be the [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) of $A$ on the [affine subspace](../../../vector-space.md#affine-subspace) $\{x:\xi\cdot x=j\}$, for $j=0,1,2$. These three [affine subspaces](../../../vector-space.md#affine-subspace) have equal [cardinality](../../../set-theory.md#cardinality), and

$$
\alpha=\frac{\alpha_0+\alpha_1+\alpha_2}{3},
\qquad
\widehat f(\xi)=\frac13\sum_{j=0}^2\alpha_j\omega^{-j},
\qquad
\alpha_j-\alpha=2\operatorname{Re}\bigl(\widehat f(\xi)\omega^j\bigr).
$$

Among three directions separated by $2\pi/3$, one makes an angle at most $\pi/3$ with any given complex number. Hence $\max_j(\alpha_j-\alpha)\geq|\widehat f(\xi)|$. Restricting to that [hyperplane](../../../vector-space.md#hyperplane) gives the [hyperplane density increment for cap sets](../../../additive-combinatorics.md#hyperplane-density-increment-for-cap-sets)

$$
\alpha'\geq\alpha+\frac{\alpha^2}{2},\qquad d'=d-1.
$$

Translate the [affine subspace](../../../vector-space.md#affine-subspace) to its underlying [vector space](../../../vector-space.md). This preserves the [cap set](../../../combinatorics.md#cap-set) property: translating a triple by $t$ changes its sum by $3t=0$. The same argument can therefore be iterated.

For completeness, the [density increment](../../../additive-combinatorics.md#density-increment) iteration gives an explicit uniform bound. If $n<16$, the hypothesis $\alpha\geq16/n$ is impossible. Suppose $n\geq16$ and a [cap set](../../../combinatorics.md#cap-set) has $\alpha_0\geq16/n$. For every integer $0\leq t\leq\lfloor n/2\rfloor$, its remaining [dimension](../../../vector-space.md#dimension-vector-space) is at least $n/2$, and its current [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) is at least $16/n$. Thus

$$
3^{n-t}\alpha_t^2\geq3^{n/2}\frac{256}{n^2}\geq2.
$$

The last inequality holds at $n=16$ and remains true as $n$ increases: the successive ratio of $3^{n/2}/n^2$ is $\sqrt3\,(n/(n+1))^2>1$ for $n\geq16$. At each step, as long as the [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) remains at most one,

$$
\frac1{\alpha_t}-\frac1{\alpha_{t+1}}
\geq\frac1{2+\alpha_t}\geq\frac13.
$$

After $L=\lfloor n/2\rfloor$ steps this would imply

$$
0<\frac1{\alpha_L}\leq\frac n{16}-\frac L3<0,
$$

a contradiction. The endpoint $\alpha=1$ already contradicts the [cap set](../../../combinatorics.md#cap-set) property in positive [dimension](../../../vector-space.md#dimension-vector-space). This proves the claimed existence of three distinct points and the [Meshulam bound for cap sets](../../../combinatorics.md#meshulam-bound-for-cap-sets).

## 2

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use uniform [expectations](../../../probability-theory.md#expected-value) on the two nonempty parts, and equip their function spaces with the [inner product](../../../linear-algebra.md#inner-product) $\langle u,v\rangle=\mathbb E\overline u v$. Let $H=G-\gamma$ and

$$
(T_Hv)(x)=\mathbb E_yH(x,y)v(y).
$$

Since the [bipartite graph](../../../graph-theory.md#bipartite-graph) is a [biregular graph](../../../graph-theory.md#biregular-graph), both row and column averages of $H$ vanish. The [normalized adjacency operator of a bipartite graph](../../../graph-theory.md#normalized-adjacency-operator-of-a-bipartite-graph) therefore splits into the map between constant functions, of [singular value](../../../linear-algebra.md#singular-value) $\gamma$, and $T_H$ between their [orthogonal complements](../../../hilbert-space.md#orthogonal-complement).

There is no [singular value](../../../linear-algebra.md#singular-value) larger than $\gamma$. Indeed, for $\gamma>0$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
|\mathbb E_yG(x,y)v(y)|^2
\leq\gamma\mathbb E_yG(x,y)|v(y)|^2.
$$

Averaging in $x$ uses the constant column degree and gives $\|\theta_Gv\|_2\leq\gamma\|v\|_2$. For $\gamma=0$ every operator is zero. Thus the second [singular value](../../../linear-algebra.md#singular-value) is

$$
s=\|T_H\|_{\mathrm{op}}.
$$

If one part has a single vertex, missing [singular values](../../../linear-algebra.md#singular-value) are interpreted as zero; the [biregular graph](../../../graph-theory.md#biregular-graph) then has $H=0$.

The discrepancy in (i) is exactly $\mathbb E H1_A1_B$. Its supremum over $A,B$ is the [cut norm](../../../additive-combinatorics.md#cut-norm) $\delta=\|H\|_{\mathrm{cut}}$. To pass from this bound to arbitrary bounded [real-valued functions](../../../function.md#real-valued-function), use the positive and negative parts and the identity $u_+(x)=\int_0^M1_{\{u(x)>t\}}\,dt$ for $|u|\leq M$. Applying this separately to both factors gives

$$
|\mathbb E_{x,y}H(x,y)u(x)v(y)|\leq4\delta MN
\quad\text{if }|u|\leq M,\ |v|\leq N.
$$

Here $N$ is a bound on $v$, unrelated to any [cardinality](../../../set-theory.md#cardinality).

If $s>0$, take real unit [left singular vector](../../../linear-algebra.md#left-singular-vector) $u$ and [right singular vector](../../../linear-algebra.md#right-singular-vector) $v$ with $T_Hv=su$ and $T_H^*u=sv$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and $|H|\leq1$ imply $\|u\|_\infty,\|v\|_\infty\leq1/s$. Hence

$$
s=\mathbb E Huv\leq\frac{4\delta}{s^2},
\qquad\boxed{s\leq(4c_1)^{1/3}}.
$$

This proves (i)$\Rightarrow$(iii), with a constant independent of both part sizes. The case $s=0$ satisfies the same conclusion immediately.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $\sigma_1=\gamma,\sigma_2,\ldots$ be the [singular values](../../../linear-algebra.md#singular-value) of the [normalized adjacency operator of a bipartite graph](../../../graph-theory.md#normalized-adjacency-operator-of-a-bipartite-graph), with the uniform [inner products](../../../linear-algebra.md#inner-product) used above. Its ordinary matrix in an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) on each side is $G/\sqrt{|X||Y|}$. Expanding the [trace](../../../linear-algebra.md#matrix-trace) of $(\theta_G\theta_G^*)^2$ proves the [box norm singular-value identity](../../../additive-combinatorics.md#box-norm-singular-value-identity)

$$
\|G\|_\square^4
=\mathbb E_{x,x',y,y'}G(x,y)G(x',y)G(x',y')G(x,y')
=\sum_j\sigma_j^4
=\gamma^4+\sum_{j\geq2}\sigma_j^4.
$$

Therefore (ii) immediately implies

$$
\boxed{s\leq c_2^{1/4}},
$$

which is (iii).

Conversely, the square of the [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm) of this operator is

$$
\sum_j\sigma_j^2=\mathbb E_{x,y}G(x,y)^2=\gamma,
$$

since a [graph](../../../graph.md) [indicator function](../../../measure-theory.md#indicator-function) takes values zero and one. Under (iii), every $\sigma_j$ with $j\geq2$ is at most $c_3$, so

$$
\sum_{j\geq2}\sigma_j^4
\leq c_3^2\sum_{j\geq2}\sigma_j^2
=c_3^2(\gamma-\gamma^2)
\leq\frac{c_3^2}{4}.
$$

Thus (iii)$\Rightarrow$(ii) with $\boxed{c_2=c_3^2/4}$. This bound also covers the empty and complete [bipartite graphs](../../../graph-theory.md#bipartite-graph).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [biregular graph](../../../graph-theory.md#biregular-graph) assumption allows both [indicator functions](../../../measure-theory.md#indicator-function) in the discrepancy to be balanced:

$$
\mathbb E_{x,y}G(x,y)1_A(x)1_B(y)-\alpha\beta\gamma
=\mathbb E_{x,y}H(x,y)(1_A(x)-\alpha)(1_B(y)-\beta).
$$

The [operator norm](../../../continuous-dual-space.md#operator-norm) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\left|\mathbb E H(1_A-\alpha)(1_B-\beta)\right|
\leq s\sqrt{\alpha(1-\alpha)\beta(1-\beta)}
\leq\frac{s}{4}.
$$

Consequently (iii)$\Rightarrow$(i) with $\boxed{c_1=c_3/4}$. Together with the previous sections, explicit constants for every direction are

$$
\begin{array}{c|cc}
\text{assumption}&\text{first consequence}&\text{second consequence}\\\hline
\text{(i), }c_1&c_3=(4c_1)^{1/3}&c_2=(4c_1)^{2/3}/4\\
\text{(ii), }c_2&c_3=c_2^{1/4}&c_1=c_2^{1/4}/4\\
\text{(iii), }c_3&c_1=c_3/4&c_2=c_3^2/4
\end{array}
$$

All these constants tend to zero with the initial constant and are independent of $|X|,|Y|$. This is the required equivalence for a [quasirandom bipartite graph](../../../graph-theory.md#quasirandom-bipartite-graph).

## 3

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the following normalization for [Fourier analysis on a finite group](../../../additive-combinatorics.md#fourier-analysis-on-a-finite-group). Choose one [unitary irreducible representation](../../../representation-theory.md#unitary-irreducible-representation) $\rho:G\to U(d_\rho)$ from each equivalence class, including the [trivial representation](../../../representation-theory.md#trivial-representation). For a scalar function $f:G\to\mathbb C$, put

$$
\widehat f(\rho)=\mathbb E_x f(x)\rho(x),
\qquad
\langle f,g\rangle=\mathbb E_x\overline{f(x)}g(x).
$$

This convention uses $\rho(x)$, rather than $\rho(x)^*$, in the [Fourier transform on a finite group](../../../additive-combinatorics.md#fourier-transform-on-a-finite-group); it makes the [normalized convolution on a finite group](../../../additive-combinatorics.md#normalized-convolution-on-a-finite-group) preserve multiplication order.

The needed [representation theory](../../../representation-theory.md) consists of [Maschke's theorem](../../../representation-theory.md#maschke-s-theorem) and [unitarization of a finite-group representation](../../../representation-theory.md#unitarization-of-a-finite-group-representation), together with the [Schur orthogonality relations](../../../representation-theory.md#schur-orthogonality-relations):

$$
\mathbb E_x\rho(x)_{ij}\overline{\sigma(x)_{kl}}
=\begin{cases}d_\rho^{-1}\delta_{ik}\delta_{jl},&\rho=\sigma,\\0,&\rho\ne\sigma.\end{cases}
$$

The [regular representation](../../../representation-theory.md#regular-representation) contains $d_\rho$ copies of each $\rho$, so $\sum_\rho d_\rho^2=|G|$. Thus the scaled [matrix coefficients](../../../representation-theory.md#matrix-coefficient) $\sqrt{d_\rho}\rho(x)_{ij}$, and also their [complex conjugates](../../../complex-analysis.md#complex-conjugate), form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of all scalar functions on $G$. These facts imply [Fourier inversion on a finite group](../../../additive-combinatorics.md#fourier-inversion-on-a-finite-group) and the [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) in the forms

$$
f(x)=\sum_\rho d_\rho\operatorname{tr}\bigl(\widehat f(\rho)\rho(x)^*\bigr),
\qquad
\langle f,g\rangle
=\sum_\rho d_\rho\operatorname{tr}\bigl(\widehat f(\rho)^*\widehat g(\rho)\bigr),
$$

and hence

$$
\|f\|_2^2=\sum_\rho d_\rho\|\widehat f(\rho)\|_{\mathrm{HS}}^2.
$$

In particular, the transform is an isomorphism onto the direct sum of the [matrix algebras](../../../associative-algebra.md#matrix-algebra) $M_{d_\rho}(\mathbb C)$, with the displayed weighted [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product).

Define the [normalized convolution on a finite group](../../../additive-combinatorics.md#normalized-convolution-on-a-finite-group) by

$$
(f*g)(x)=\mathbb E_yf(y)g(y^{-1}x).
$$

Substituting $x=yz$ and using the [group representation](../../../representation-theory.md#group-representation) identity yields the [convolution theorem on a finite group](../../../additive-combinatorics.md#convolution-theorem-on-a-finite-group)

$$
\widehat{f*g}(\rho)=\widehat f(\rho)\widehat g(\rho).
$$

Unlike [normalized convolution on a finite group](../../../additive-combinatorics.md#normalized-convolution-on-a-finite-group) on an [abelian group](../../../group.md#abelian-group), this product need not commute. If $\widetilde f(x)=\overline{f(x^{-1})}$, then $\widehat{\widetilde f}(\rho)=\widehat f(\rho)^*$. For [left translation of a group function](../../../additive-combinatorics.md#left-translation-of-a-group-function) and [right translation of a group function](../../../additive-combinatorics.md#right-translation-of-a-group-function) $L_af(x)=f(a^{-1}x)$ and $R_af(x)=f(xa)$,

$$
\widehat{L_af}(\rho)=\rho(a)\widehat f(\rho),
\qquad
\widehat{R_af}(\rho)=\widehat f(\rho)\rho(a)^*.
$$

For an [abelian group](../../../group.md#abelian-group), every [irreducible representation](../../../representation-theory.md#irreducible-representation) is one-dimensional; this reduces to [Fourier analysis on a finite abelian group](../../../additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group) with characters relabelled by their inverses. These formulas establish the basic scalar theory, with all normalizations and multiplication orders fixed.

Now suppose every nontrivial [irreducible representation](../../../representation-theory.md#irreducible-representation) has $d_\rho\geq m$. If $f$ is a [mean-zero function](../../../probability-theory.md#mean-zero-function), its component at the [trivial representation](../../../representation-theory.md#trivial-representation) is zero. The [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) gives, for each other $\rho$,

$$
\|\widehat f(\rho)\|_{\mathrm{op}}
\leq\|\widehat f(\rho)\|_{\mathrm{HS}}
\leq\frac{\|f\|_2}{\sqrt{d_\rho}}
\leq\frac{\|f\|_2}{\sqrt m}.
$$

Using the [convolution theorem on a finite group](../../../additive-combinatorics.md#convolution-theorem-on-a-finite-group), the [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm) inequality $\|AB\|_{\mathrm{HS}}\leq\|A\|_{\mathrm{op}}\|B\|_{\mathrm{HS}}$, and the [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) once more gives the [product mixing in a quasirandom group](../../../additive-combinatorics.md#product-mixing-in-a-quasirandom-group) estimate

$$
\boxed{\|f*g\|_2\leq m^{-1/2}\|f\|_2\|g\|_2\quad\text{when }\mathbb E f=0.}
$$

Write $a,b,c$ for the [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) values of $A,B,C$, respectively, and let $f=1_A-a$, $g=1_B-b$ be [balanced subset indicators](../../../additive-combinatorics.md#balanced-indicator-function-of-a-finite-subset). Since both are [mean-zero functions](../../../probability-theory.md#mean-zero-function), $1_A*1_B=ab+f*g$. Their squared [norms](../../../functional-analysis.md#norm) are $a(1-a)$ and $b(1-b)$. Also $\mathbb E(f*g)=0$, so the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) yields

$$
\begin{aligned}
\left|\mathbb E_z(1_A*1_B)(z)1_C(z)-abc\right|
&=\left|\mathbb E_z(f*g)(z)(1_C(z)-c)\right|\\
&\leq\sqrt{\frac{a(1-a)b(1-b)c(1-c)}m}
\leq\sqrt{\frac{abc}{m}}.
\end{aligned}
$$

If $abc>1/m$, the final bound is strictly smaller than $abc$. Thus the normalized number of pairs $(x,y)\in A\times B$ with $xy\in C$ is positive. Equivalently,

$$
\boxed{|A||B||C|>|G|^3/m\ \Longrightarrow\ AB\cap C\ne\varnothing.}
$$

This is the desired conclusion for a [quasirandom group](../../../additive-combinatorics.md#quasirandom-group); the strict inequality ensures positivity rather than merely a nonnegative lower bound.

## 4

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Use $c>0$, the necessary parameter range for the bounds involving $1/c$. The construction comes from the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of [matrix Fourier blocks](../../../additive-combinatorics.md#matrix-fourier-block). For each inequivalent [unitary irreducible representation](../../../representation-theory.md#unitary-irreducible-representation) $\rho$ of [dimension](../../../vector-space.md#dimension-vector-space) $d_\rho$, consider the [Hilbert space](../../../hilbert-space.md) $\mathcal H_\rho=M_{n\times d_\rho}(\mathbb C)$ with the [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) $\langle A,B\rangle=\operatorname{tr}(A^*B)$ and the operator

$$
T_\rho(A)=\mathbb E_x f(x)A\rho(x)^*.
$$

Its [operator norm](../../../continuous-dual-space.md#operator-norm) is at most one, since $\rho(x)$ is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) and $\|f(x)\|_{\mathrm{op}}\leq1$. Thus all its [singular values](../../../linear-algebra.md#singular-value) $\lambda_{\rho,j}$ lie in $[0,1]$.

Two identities control their weighted moments:

$$
S_2=\sum_\rho d_\rho\sum_j\lambda_{\rho,j}^2
=\mathbb E_x\operatorname{tr}(f(x)f(x)^*)\leq n,
$$



$$
S_4=\sum_\rho d_\rho\sum_j\lambda_{\rho,j}^4
=\mathbb E_{xy^{-1}zw^{-1}=e}\operatorname{tr}(f(x)f(y)^*f(z)f(w)^*)\geq cn.
$$

Here the [expectation](../../../probability-theory.md#expected-value) in $S_4$ is uniform on the $|G|^3$ solutions of the constraint, and the [trace](../../../linear-algebra.md#matrix-trace) on $\mathcal H_\rho$ used to compute each moment is the ordinary operator [trace](../../../linear-algebra.md#matrix-trace). We justify the identities explicitly to fix their normalizations and the noncommutative order.

The [adjoint operator](../../../hilbert-space.md#adjoint-operator) is $T_\rho^*(A)=\mathbb E_yf(y)^*A\rho(y)$, so

$$
T_\rho T_\rho^*(A)
=\mathbb E_{x,y}f(x)f(y)^*A\rho(yx^{-1}).
$$

For rectangular matrices, the operator $A\mapsto LAR$ has [trace](../../../linear-algebra.md#matrix-trace) $\operatorname{tr}(L)\operatorname{tr}(R)$, as is seen on the matrix-unit [basis](../../../vector-space.md#basis). Squaring the previous operator therefore gives

$$
\begin{aligned}
\operatorname{Tr}_{\mathcal H_\rho}(T_\rho T_\rho^*)&=\mathbb E_{x,y}\operatorname{tr}(f(x)f(y)^*)\chi_\rho(yx^{-1}),\\
\operatorname{Tr}_{\mathcal H_\rho}((T_\rho T_\rho^*)^2)&=\mathbb E_{x,y,z,w}\operatorname{tr}(f(x)f(y)^*f(z)f(w)^*)\chi_\rho(wz^{-1}yx^{-1}).
\end{aligned}
$$

The required [representation theory](../../../representation-theory.md) consists of [unitarization of a finite-group representation](../../../representation-theory.md#unitarization-of-a-finite-group-representation), the [Schur orthogonality relations](../../../representation-theory.md#schur-orthogonality-relations), and the [regular representation](../../../representation-theory.md#regular-representation) decomposition. The last gives the [character expansion of the identity delta](../../../representation-theory.md#character-expansion-of-the-identity-delta)

$$
\sum_\rho d_\rho\chi_\rho(g)=|G|1_{\{g=e\}}.
$$

Summing the two operator [traces](../../../linear-algebra.md#matrix-trace) with weights $d_\rho$ selects $x=y$ in the first, and $w=xy^{-1}z$ in the second. Multiplication by $|G|$ converts each independent-variable [expectation](../../../probability-theory.md#expected-value) to its conditional [expectation](../../../probability-theory.md#expected-value). This proves $S_2,S_4$. In particular $S_4$ is real and nonnegative, despite the apparently complex summands in its original formula. Since $S_4\leq S_2\leq n$, the nonvacuous hypothesis has $0<c\leq1$.

Select every [singular value](../../../linear-algebra.md#singular-value) satisfying $\lambda_{\rho,j}\geq\sqrt{c/2}$. Index the selected pairs by $p=1,\ldots,r$, set $\rho_p=\rho$, $n_p=d_\rho$, and choose unit [right singular vectors](../../../linear-algebra.md#right-singular-vector) $A_p$ and unit [left singular vectors](../../../linear-algebra.md#left-singular-vector) $B_p$ with $T_{\rho_p}A_p=\lambda_pB_p$. Define

$$
\boxed{U(p)=\sqrt{n_p}A_p,\qquad V(p)=\sqrt{n_p}B_p.}
$$

Both are $n\times n_p$ matrices, proving (i). Repeated [group representations](../../../representation-theory.md#group-representation) in this list are literally the same chosen representative, rather than different equivalent realizations.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The [singular values](../../../linear-algebra.md#singular-value) discarded by the threshold in (i) satisfy $\lambda^2<c/2$, so their contribution to the fourth moment is at most $(c/2)S_2\leq cn/2$. The selected [singular values](../../../linear-algebra.md#singular-value) consequently satisfy

$$
\sum_{p=1}^r n_p\lambda_p^4\geq cn/2.
$$

Because $\lambda_p\leq1$, this implies $m=\sum_pn_p\geq cn/2$. On the other hand, $\lambda_p^2\geq c/2$, and hence

$$
\frac c2\,m\leq\sum_pn_p\lambda_p^2\leq S_2\leq n.
$$

Thus

$$
\boxed{\frac{cn}{2}\leq m\leq\frac{2n}{c}}.
$$

The lower bound also shows that the selected list is nonempty. Both endpoints are inclusive, as required.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The selected [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) directly gives

$$
\mathbb E_x f(x)U(p)\rho_p(x)^*
=T_{\rho_p}(U(p))
=\lambda_pV(p),
\qquad\boxed{\sqrt{c/2}\leq\lambda_p\leq1}.
$$

Each $\lambda_p$ is a real nonnegative [singular value](../../../linear-algebra.md#singular-value). The scale factor $\sqrt{n_p}$ in both matrices cancels in this equation and is chosen to give the precise [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) normalization in (iv).

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Within each fixed [unitary irreducible representation](../../../representation-theory.md#unitary-irreducible-representation), choose the selected [right singular vectors](../../../linear-algebra.md#right-singular-vector) to be [orthonormal](../../../linear-algebra.md#orthonormal-set). Their corresponding [left singular vectors](../../../linear-algebra.md#left-singular-vector) are also [orthonormal](../../../linear-algebra.md#orthonormal-set), even when a [singular value](../../../linear-algebra.md#singular-value) is repeated: choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) in each eigenspace of $T_\rho^*T_\rho$ and put $B_p=T_\rho A_p/\lambda_p$. Therefore, when $\rho_p=\rho_q$,

$$
\boxed{\operatorname{tr}(U(p)^*U(q))
=\operatorname{tr}(V(p)^*V(q))
=n_p\delta_{pq}}.
$$

This is (iv), with the unnormalized [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) and the [Kronecker delta](../../../linear-algebra.md#kronecker-delta). No orthogonality of differently shaped matrices is being asserted.

For the unheaded continuation, partition $b\in\mathbb C^m$ into blocks $b_p\in\mathbb C^{n_p}$. Then

$$
UP(x)^*b=\sum_pU(p)\rho_p(x)^*b_p.
$$

The [Schur averaging of rectangular matrices](../../../representation-theory.md#schur-averaging-of-rectangular-matrices) formula is

$$
\mathbb E_x\rho_p(x)M\rho_q(x)^*
=\begin{cases}(\operatorname{tr}M/n_p)I_{n_p},&\rho_p=\rho_q,\\0,&\rho_p\ne\rho_q,\end{cases}
$$

for any $n_p\times n_q$ matrix $M$. The average is an [intertwiner](../../../representation-theory.md#intertwiner); the [Schur lemma](../../../representation-theory.md#schur-s-lemma) makes it zero for inequivalent [irreducible representations](../../../representation-theory.md#irreducible-representation), and a scalar multiple of the identity for the same representative. The [trace](../../../linear-algebra.md#matrix-trace) determines that scalar in the latter case.

Apply this with $M=U(p)^*U(q)$. The [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) normalization just proved gives

$$
\mathbb E_x\rho_p(x)U(p)^*U(q)\rho_q(x)^*
=\begin{cases}I_{n_p},&p=q,\\0,&p\ne q.\end{cases}
$$

Expanding the squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) now yields

$$
\begin{aligned}
\mathbb E_x\|UP(x)^*b\|_2^2
&=\sum_{p,q}b_p^*\mathbb E_x\bigl[\rho_p(x)U(p)^*U(q)\rho_q(x)^*\bigr]b_q\\
&=\sum_p\|b_p\|_2^2
=\boxed{\|b\|_2^2}.
\end{aligned}
$$

Thus the final identity follows from averaging, although $U^*U$ itself need not be the identity. The whole construction is the [spectral inverse theorem for the matrix-valued U2 quantity](../../../additive-combinatorics.md#spectral-inverse-theorem-for-the-matrix-valued-u2-quantity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
