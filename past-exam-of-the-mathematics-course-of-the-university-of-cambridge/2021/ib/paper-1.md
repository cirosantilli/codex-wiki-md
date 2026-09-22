# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperib_1_2021.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperib_1_2021.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6H](#6h)
  - [a](#6h/a)
    - [Solution](#6h/a/solution)
  - [b](#6h/b)
    - [Solution](#6h/b/solution)
  - [c](#6h/c)
    - [Solution](#6h/c/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
  - [c](#7h/c)
    - [Solution](#7h/c/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [i](#8e/a/i)
      - [Solution](#8e/a/i/solution)
    - [ii](#8e/a/ii)
      - [Solution](#8e/a/ii/solution)
  - [b](#8e/b)
    - [i](#8e/b/i)
      - [Solution](#8e/b/i/solution)
    - [ii](#8e/b/ii)
      - [Solution](#8e/b/ii/solution)
    - [iii](#8e/b/iii)
      - [Solution](#8e/b/iii/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10F](#10f)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
  - [d](#10f/d)
    - [Solution](#10f/d/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12G](#12g)
  - [a](#12g/a)
    - [Solution](#12g/a/solution)
  - [b](#12g/b)
    - [Solution](#12g/b/solution)
  - [c](#12g/c)
    - [Solution](#12g/c/solution)
- [13C](#13c)
  - [a](#13c/a)
    - [Solution](#13c/a/solution)
  - [b](#13c/b)
    - [Solution](#13c/b/solution)
- [14C](#14c)
  - [i](#14c/i)
    - [Solution](#14c/i/solution)
  - [ii](#14c/ii)
    - [Solution](#14c/ii/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [Solution](#15d/b/solution)
  - [c](#15d/c)
    - [Solution](#15d/c/solution)
- [16A](#16a)
  - [a](#16a/a)
    - [Solution](#16a/a/solution)
  - [b](#16a/b)
    - [Solution](#16a/b/solution)
  - [c](#16a/c)
    - [Solution](#16a/c/solution)
- [17B](#17b)
  - [i](#17b/i)
    - [Solution](#17b/i/solution)
  - [ii](#17b/ii)
    - [Solution](#17b/ii/solution)
  - [iii](#17b/iii)
    - [Solution](#17b/iii/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)

## 1E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The map

$$
\ell_v:V\to\mathbb R,
\qquad
\ell_v(x)=\langle v,x\rangle
$$

is a nonzero [linear functional](../../../linear-algebra.md#linear-functional): otherwise $v$ would lie in the [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form), contradicting nondegeneracy. Its kernel is $v^\perp$, so the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives $\dim v^\perp=n-1$. Antisymmetry gives $\langle v,v\rangle=-\langle v,v\rangle=0$, hence $v\in v^\perp$.

Suppose $w\in W$ is orthogonal to every vector of $W$. Since $W\subseteq v^\perp$, it is also orthogonal to $v$, and therefore to

$$
W\oplus\mathbb Rv=v^\perp.
$$

For a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form), $(v^\perp)^\perp=\mathbb Rv$: both sides have dimension one and the latter is contained in the former. Thus $w\in W\cap\mathbb Rv=\{0\}$, proving that the restriction to $W$ is nondegenerate.

The space $W$ has dimension $n-2$ and again carries a nondegenerate antisymmetric form. Induction, starting from the zero-dimensional space, shows that $\dim W$ is even. Therefore $n=\dim W+2$ is even. Equivalently, every finite-dimensional [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) has even dimension.

## 2F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

The condition $Df_p\ne0$ says that $0$ is a [regular value](../../../differential-geometry.md#regular-value) of $f$. The [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) therefore makes $f^{-1}(0)$ a smooth submanifold of codimension one in $\mathbb R^3$, hence a [smooth surface](../../../differential-geometry.md#smooth-surface).

For

$$
F(x,y,z)=x^2+y^2-\cosh(z^2),
$$

the [gradient](../../../calculus.md#gradient) is

$$
\nabla F=(2x,2y,-2z\sinh(z^2)).
$$

On $F^{-1}(0)$, $x^2+y^2=\cosh(z^2)\geq1$, so $x$ and $y$ cannot both vanish. Thus $\nabla F\ne0$ there, and the given set is a smooth surface.

Not every smooth surface in $\mathbb R^3$ is a global zero set. Every set $f^{-1}(0)$ is [closed](../../../topology.md#closed-set) because $f$ is continuous, whereas the open unit disk

$$
\{(x,y,0):x^2+y^2<1\}
$$

is a smooth surface but is not closed in $\mathbb R^3$.

## 3B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

The integrand has an order-two [pole](../../../isolated-singularity.md#pole) at $0$ and a simple pole at $2$. Write it near zero as $h(z)/z^2$, where

$$
h(z)=\frac{z^2+e^z}{z-2}.
$$

Its [residue](../../../analysis.md#residue) at zero is

$$
h'(0)=\left.\frac{(2z+e^z)(z-2)-(z^2+e^z)}{(z-2)^2}\right|_{z=0}
=-\frac34.
$$

At $z=2$ the residue is

$$
\frac{2^2+e^2}{2^2}=1+\frac{e^2}{4}.
$$

The [residue theorem](../../../analysis.md#residue-theorem) now gives

$$
\boxed{
g(x)=\begin{cases}
-\dfrac{3\pi i}{2},&0<x<2,\\[4pt]
\dfrac{\pi i}{2}(1+e^2),&x>2.
\end{cases}}
$$

## 4D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

Introduce a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\lambda$ for the normalization and vary

$$
J[u]=\int_D\bigl(|\nabla u|^2-\lambda u^2\bigr)\,dx\,dy.
$$

For a smooth variation $u+\varepsilon\eta$ with $\eta=0$ on $\partial D$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\left.\frac d{d\varepsilon}J[u+\varepsilon\eta]\right|_{\varepsilon=0}
=2\int_D(\nabla u\mathbin{\cdot}\nabla\eta-\lambda u\eta)
=-2\int_D(\nabla^2u+\lambda u)\eta.
$$

The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore yields the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\boxed{\nabla^2u+\lambda u=0}.
$$

Multiplying by $u$ and integrating, while using

$$
\nabla\mathbin{\cdot}(u\nabla u)=|\nabla u|^2+u\nabla^2u,
$$

the [divergence theorem](../../../calculus.md#divergence-theorem) and $u=0$ on the boundary give

$$
0=I[u]+\int_Du\nabla^2u=I[u]-\lambda\int_Du^2.
$$

The normalization is one, so the multiplier equals the stationary value:

$$
\boxed{\lambda=I[u]}.
$$

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Apply symmetric [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) without row exchanges. At step $k$, let $d_k$ be the leading diagonal entry of the remaining symmetric [Schur complement](../../../linear-algebra.md#schur-complement). If $d_k\leq0$, stop and report that $A$ is not [positive definite](../../../linear-algebra.md#positive-definite-matrix). If $d_k>0$, use it to eliminate the rest of its row and column. If all steps succeed, this constructs an [LDL decomposition](../../../numerical-analysis.md#ldl-decomposition)

$$
A=LDL^T,
$$

where $L$ is unit lower triangular and $D=\operatorname{diag}(d_1,\ldots,d_n)$ has positive diagonal.

The test is correct from first principles. If all $d_k>0$, then for every nonzero $x$,

$$
x^TAx=(L^Tx)^TD(L^Tx)>0
$$

because $L$ is invertible. Conversely, if $A$ is positive definite, its first pivot is $a_{11}>0$, and completing the square gives

$$
\begin{pmatrix}s\\y\end{pmatrix}^{T}
\begin{pmatrix}a&b^T\\b&C\end{pmatrix}
\begin{pmatrix}s\\y\end{pmatrix}
=a\left(s+\frac{b^Ty}{a}\right)^2
+y^T\left(C-\frac{bb^T}{a}\right)y.
$$

Choosing $s=-b^Ty/a$ shows that the Schur complement is positive definite. Induction forces every pivot to be positive. This is also [Sylvester's criterion](../../../linear-algebra.md#sylvester-s-criterion).

At step $k$, updating the remaining matrix costs $O((n-k)^2)$ arithmetic operations. Hence the total is

$$
\sum_{k=1}^nO((n-k)^2)=O(n^3),
$$

which proves the existence of the required algorithm.

## 6H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6h/a">a</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/a/solution">Solution</h4>

↑ **Parent:** [A](#6h/a)

A [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) $T$ is one for which the conditional distribution of the full sample $(X_1,\ldots,X_n)$ given $T$ does not depend on $p$. Take

$$
T=\sum_{i=1}^nX_i.
$$

For a binary sample $x$ with $\sum_i x_i=t$, its [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
p^t(1-p)^{n-t},
$$

which depends on the data only through $t$. By the [Fisher-Neyman factorization theorem](../../../probability-and-statistics.md#fisher-neyman-factorization-theorem), $T$ is sufficient. Equivalently, conditionally on $T=t$, the sample is uniform over the $\binom nt$ binary vectors containing $t$ ones, independently of $p$.

<h3 id="6h/b">b</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/b/solution">Solution</h4>

↑ **Parent:** [B](#6h/b)

The [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) states that if $T$ is sufficient and $U$ is an estimator with finite variance, then

$$
U^*=\mathbb E[U\mid T]
$$

has the same expectation as $U$ and no larger variance; it preserves unbiasedness. The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E U^*=\mathbb E U.
$$

The [law of total variance](../../../probability-theory.md#law-of-total-variance) gives

$$
\operatorname{Var}(U)
=\operatorname{Var}(\mathbb E[U\mid T])
+\mathbb E[\operatorname{Var}(U\mid T)]
\geq\operatorname{Var}(U^*).
$$

Sufficiency ensures that $U^*$ is a statistic whose definition does not depend on the unknown parameter. The inequality is strict exactly when the conditional variance is positive with positive probability.

<h3 id="6h/c">c</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/c/solution">Solution</h4>

↑ **Parent:** [C](#6h/c)

The estimator $U=X_1X_2$ is [unbiased](../../../statistical-modelling.md#unbiased-estimator) for $p^2$ because the [independent random variables](../../../random-variable.md#independent-random-variables) $X_1,X_2$ satisfy $\mathbb E[X_1X_2]=p^2$. Given $T=t$, all placements of the $t$ successes are equally likely, so

$$
\mathbb E[X_1X_2\mid T=t]
=\frac{\binom{n-2}{t-2}}{\binom nt}
=\frac{t(t-1)}{n(n-1)}.
$$

Thus the Rao-Blackwellized estimator is

$$
\boxed{\widehat{p^2}=\frac{T(T-1)}{n(n-1)}}.
$$

It is unbiased by the tower property. Since $n\geq3$ and $p\in(0,1)$, the event $T=2$ has positive probability, and conditionally on it $X_1X_2$ takes both zero and one with positive probability. Hence $\mathbb E[\operatorname{Var}(X_1X_2\mid T)]>0$, so the new estimator has strictly smaller variance.

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

For $0\leq t\leq1$ and $x,y\in\mathbb R^d$, [convexity](../../../real-analysis.md#convex-function) gives

$$
f_i(tx+(1-t)y)\leq tf_i(x)+(1-t)f_i(y).
$$

Taking the maximum over $i$ and then bounding each term by the corresponding endpoint maxima yields

$$
\max_i f_i(tx+(1-t)y)
\leq t\max_i f_i(x)+(1-t)\max_i f_i(y).
$$

**Thus the finite [pointwise maximum of convex functions](../../../real-analysis.md#pointwise-maximum-of-convex-functions) is convex. Summing the original inequalities over $i$ proves that $\sum_i f_i$ is convex as well.**

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

Because $x\mapsto c^Tx$ is a [linear map](../../../vector-space.md#linear-map),

$$
g(tx+(1-t)y)
=f(tc^Tx+(1-t)c^Ty)
\leq tf(c^Tx)+(1-t)f(c^Ty).
$$

**Hence composition of a convex function with an affine map is convex, and $g$ is convex.**

<h3 id="7h/c">c</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/c/solution">Solution</h4>

↑ **Parent:** [C](#7h/c)

The [softplus function](../../../real-analysis.md#softplus)

$$
h(s)=\log(1+e^s)
$$

is convex because

$$
h''(s)=\frac{e^s}{(1+e^s)^2}\geq0.
$$

Part (b) therefore shows that every $\beta\mapsto h(a_i^T\beta)$ is convex. The [absolute value function](../../../real-analysis.md#absolute-value) is convex, so $\beta\mapsto|\beta_j|$ is convex for every coordinate $j$. Finally, part (a) says that a finite sum of convex functions is convex. Therefore

$$
Q(\beta)=\sum_{i=1}^n\log(1+e^{a_i^T\beta})+\sum_{j=1}^d|\beta_j|
$$

is convex. The second sum is the [L1 norm](../../../functional-analysis.md#l1-norm) regularizer.

## 8E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/i">i</h4>

↑ **Parent:** [A](#8e/a)

<h5 id="8e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8e/a/i)

The [Nilpotent Jordan block](../../../linear-operator-theory.md#nilpotent-jordan-block) $J_d$ shifts each standard basis vector one place toward the first coordinate. Therefore

$$
(J_d^n)_{ij}
=\begin{cases}
1,&j-i=n,\\
0,&\text{otherwise}.
\end{cases}
$$

Thus $J_d^0=I$, for $1\leq n<d$ the matrix has ones precisely on its $n$th superdiagonal, and

$$
\boxed{J_d^n=0\quad\text{for }n\geq d}.
$$

<h4 id="8e/a/ii">ii</h4>

↑ **Parent:** [A](#8e/a)

<h5 id="8e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8e/a/ii)

Since $\lambda I$ commutes with $J_d$, the [binomial theorem for commuting matrices](../../../combinatorics.md#binomial-theorem-for-commuting-matrices) and part (i) give

$$
\boxed{(\lambda I+J_d)^n
=\sum_{k=0}^{\min(n,d-1)}
\binom nk\lambda^{\,n-k}J_d^k}.
$$

Equivalently, its $k$th superdiagonal is constant with value $\binom nk\lambda^{n-k}$ for $0\leq k<d$, with the convention that this value is zero when $k>n$.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/i">i</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8e/b/i)

If $\phi v=\mu v$ for a nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$, then

$$
0=\phi^nv=\mu^nv.
$$

**Hence every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) satisfies $\mu=0$. Since a complex endomorphism has an eigenvalue, zero is the only possible eigenvalue.**

<h4 id="8e/b/ii">ii</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8e/b/ii)

The [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) can contain only blocks $J_r(0)$ with eigenvalue zero. Moreover,

$$
J_r(0)^n=0
\quad\Longleftrightarrow\quad r\leq n.
$$

**Thus the possible blocks are precisely the nilpotent Jordan blocks of sizes $1\leq r\leq n$.**

<h4 id="8e/b/iii">iii</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8e/b/iii)

Assume $\phi^2=0$. Then

$$
\operatorname{im}\phi\subseteq\ker\phi.
$$

Set $W_1=\operatorname{im}\phi$, choose a [direct-sum complement](../../../vector-space.md#direct-sum-complement) $U$ such that $\ker\phi=U\oplus W_1$, and choose a complement $W_2$ such that $V=\ker\phi\oplus W_2$.

The restriction $\phi|_{W_2}:W_2\to W_1$ is injective because $W_2\cap\ker\phi=0$, and it is surjective because every image $\phi(v)$ equals $\phi(w_2)$ after decomposing $v=k+w_2$. It is therefore a [isomorphism](../../../vector-space.md#linear-isomorphism), so $\dim W_2=\dim W_1$ and $\phi(W_2)=W_1$. Also $\phi(U)=\phi(W_1)=0$. Hence

$$
\boxed{V=U\oplus W_1\oplus W_2}
$$

has all the required properties.

## 9G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

Suppose first that every [ideal](../../../commutative-algebra.md#ideal) of $R$ is finitely generated. For an ascending chain

$$
I_1\subseteq I_2\subseteq\cdots,
$$

the union $I=\bigcup_nI_n$ is an ideal. Its finite generating set lies in one $I_N$, so $I_n=I_N$ for all $n\geq N$. Thus $R$ satisfies the [ascending chain condition](../../../algebra.md#ascending-chain-condition) and is a [Noetherian ring](../../../algebra.md#noetherian-ring).

Conversely, if an ideal $I$ is not finitely generated, choose $a_1\in I$, and after choosing $a_1,\ldots,a_n$, choose

$$
a_{n+1}\in I\setminus(a_1,\ldots,a_n).
$$

This creates a strictly ascending chain of ideals, contradicting Noetherianity. Hence every ideal is finitely generated.

If $\varphi:R\to S$ is surjective and $J\lhd S$, then $\varphi^{-1}(J)$ is an ideal of $R$. If it is generated by $a_1,\ldots,a_m$, then $J$ is generated by $\varphi(a_1),\ldots,\varphi(a_m)$. Thus every ideal of $S$ is finitely generated, so $S$ is Noetherian.

The [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem) states that if $R$ is a commutative Noetherian ring, then $R[X]$ is Noetherian. To prove it, let $I\lhd R[X]$. The leading coefficients of polynomials in $I$ generate an ideal of $R$; choose generators that occur as leading coefficients of $f_1,\ldots,f_s\in I$, and let $N=\max_i\deg f_i$. For each degree below $N$, the leading coefficients of members of $I$ of at most that degree likewise form a finitely generated ideal; choose finitely many corresponding polynomials. Any $f\in I$ of degree at least $N$ can have its leading term cancelled by a linear combination of monomial multiples of the $f_i$. Repeating lowers its degree below $N$, where the second finite list completes the reduction. These finitely many selected polynomials generate $I$, proving the theorem.

For every $\alpha\in\mathbb C$, the ring $\mathbb Z[\alpha]$ is Noetherian. If $\alpha$ is transcendental, evaluation identifies it with $\mathbb Z[X]$. If $\alpha$ is algebraic, it is a quotient of $\mathbb Z[X]$. The integers are Noetherian, the Hilbert basis theorem handles $\mathbb Z[X]$, and quotients preserve Noetherianity.

For a [unique factorization domain](../../../algebra.md#unique-factorization-domain) that is not Noetherian, take

$$
k[x_1,x_2,\ldots].
$$

Every polynomial and every factorization uses only finitely many variables, so existence and uniqueness of factorization reduce to a finite-variable polynomial ring, which is a UFD. But

$$
(x_1)\subsetneq(x_1,x_2)\subsetneq(x_1,x_2,x_3)\subsetneq\cdots
$$

is a strictly ascending chain, so the ring is not Noetherian.

Finally, the ring $C(\mathbb R,\mathbb R)$ is not Noetherian. For $n\geq1$, let

$$
I_n=\{f:f(x)=0\text{ for all }|x|\leq1/n\}.
$$

These are ideals and $I_n\subsetneq I_{n+1}$: the distance function to $[-1/(n+1),1/(n+1)]$ belongs to $I_{n+1}$ but not to $I_n$. This strict ascending chain proves the claim.

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

Assume inverse images of [open sets](../../../topology.md#open-set) are open. If $x_n\to a$ and $V$ is any open neighbourhood of $f(a)$, then $f^{-1}(V)$ is an open neighbourhood of $a$. By the definition of [convergence in a metric space](../../../topological-analysis.md#convergence-in-a-metric-space), $x_n\in f^{-1}(V)$ eventually, and hence $f(x_n)\in V$ eventually. Thus $f(x_n)\to f(a)$.

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

Assume the sequential condition, and let $A\subseteq Y$ be open. If $f^{-1}(A)$ were not open, some $a\in f^{-1}(A)$ would have no ball contained in $f^{-1}(A)$. For each $n$, choose

$$
x_n\notin f^{-1}(A),
\qquad
d_X(x_n,a)<\frac1n.
$$

Then $x_n\to a$, so $f(x_n)\to f(a)\in A$. Because $A$ is open, this forces $f(x_n)\in A$ eventually, a contradiction. Therefore $f^{-1}(A)$ is open. This proves the [sequential characterization of continuity in metric spaces](../../../topological-analysis.md#sequential-characterization-of-continuity-in-metric-spaces).

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

This is always true: it is the [Heine-Cantor theorem](../../../topological-analysis.md#heine-cantor-theorem). If uniform continuity failed, there would be an $\varepsilon>0$ and sequences $x_n,y_n\in X$ such that

$$
d_X(x_n,y_n)<\frac1n,
\qquad
d_Y(f(x_n),f(y_n))\geq\varepsilon.
$$

By [sequential compactness of a compact metric space](../../../topological-analysis.md#sequential-compactness-of-a-compact-metric-space), some subsequence $x_{n_k}$ converges to $x\in X$. The triangle inequality gives $y_{n_k}\to x$. Continuity then makes both image subsequences converge to $f(x)$, contradicting their separation by $\varepsilon$.

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

This may be false because continuity only forces the [continuous image of a compact space](../../../topology.md#continuous-image-of-a-compact-space) $f(X)$ to be compact, not the whole codomain. For example, let $X=\{0\}$, let $Y=\mathbb R$, and set $f(0)=0$. The domain is compact and $f$ is continuous, but $\mathbb R$ is not compact.

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

This is always true. The continuous image $f(X)$ of a [connected space](../../../geometry-and-topology.md#connected-space) is connected. Its [closure](../../../topology.md#closure-topology) is also connected: if the closure were separated into disjoint nonempty relatively open sets, connectedness would put $f(X)$ inside one of them, preventing its closure from meeting the other. Since $f(X)$ is dense in $Y$, its closure is $Y$, so $Y$ is connected.

<h3 id="10f/d">d</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/d/solution">Solution</h4>

↑ **Parent:** [D](#10f/d)

This is always true for metric spaces. Let $x_n\to x$. If $f(x_n)$ did not converge to $f(x)$, some subsequence would remain at least $\varepsilon>0$ from $f(x)$. Compactness of $Y$ gives a further subsequence

$$
f(x_{n_k})\to y.
$$

Then $(x_{n_k},f(x_{n_k}))\to(x,y)$. The graph is closed, so $(x,y)$ belongs to it and $y=f(x)$, contradicting the $\varepsilon$ separation. Thus $f(x_n)\to f(x)$ for every convergent sequence, and the equivalence proved above makes $f$ continuous. This is the [closed-graph criterion with compact codomain](../../../topology.md#closed-graph-criterion-with-compact-codomain).

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

For an oriented [smooth surface](../../../differential-geometry.md#smooth-surface) $S$, the [Gauss map](../../../differential-geometry.md#gauss-map) sends $p$ to the chosen unit [normal vector](../../../differential-geometry.md#normal-vector) $N(p)\in S^2$. Since $|N|^2=1$, differentiation shows that $DN_p(X)$ is perpendicular to $N(p)$ and hence lies in $T_pS$.

In a local parametrization $\phi(u,v)$ with $n=N\circ\phi$, differentiating

$$
n\mathbin{\cdot}\phi_u=n\mathbin{\cdot}\phi_v=0
$$

gives

$$
n_u\mathbin{\cdot}\phi_v=-n\mathbin{\cdot}\phi_{uv}
=n_v\mathbin{\cdot}\phi_u.
$$

Thus the bilinear form $(X,Y)\mapsto DN_p(X)\mathbin{\cdot}Y$ is symmetric, so $DN_p$ is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator). The [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) is

$$
\kappa=\det(DN_p).
$$

Writing the coefficients of the [first fundamental form](../../../differential-geometry.md#first-fundamental-form) as

$$
E=\phi_u^2,\qquad F=\phi_u\mathbin{\cdot}\phi_v,\qquad G=\phi_v^2
$$

and those of the [second fundamental form](../../../second-fundamental-form.md) as

$$
e=n\mathbin{\cdot}\phi_{uu},\qquad
f=n\mathbin{\cdot}\phi_{uv},\qquad
g=n\mathbin{\cdot}\phi_{vv},
$$

one obtains

$$
\boxed{\kappa=\frac{eg-f^2}{EG-F^2}}.
$$

At an [umbilic point](../../../second-fundamental-form.md#umbilical-point), the self-adjoint map $DN_p$ has a repeated eigenvalue, so it is a scalar map. If every point is umbilic, there is a function $\lambda$ with

$$
n_u=\lambda\phi_u,\qquad n_v=\lambda\phi_v.
$$

Equality of mixed partial derivatives gives

$$
\lambda_v\phi_u=\lambda_u\phi_v.
$$

The two tangent vectors are linearly independent, hence $\lambda_u=\lambda_v=0$. Since $\mathbb R^2$ is connected, $\lambda$ is constant.

If $\lambda=0$, then $n$ is constant and

$$
\partial_u(n\mathbin{\cdot}\phi)
=\partial_v(n\mathbin{\cdot}\phi)=0,
$$

so $S$ lies in a plane. If $\lambda\ne0$, then

$$
\partial_u(n-\lambda\phi)
=\partial_v(n-\lambda\phi)=0.
$$

Thus $n-\lambda\phi=c$ is constant, and

$$
\left|\phi+\frac c\lambda\right|
=\frac{|n|}{|\lambda|}
=\frac1{|\lambda|}.
$$

**Therefore $S$ lies in a sphere of radius $1/|\lambda|$. This proves that the surface is part of a plane or part of a sphere.**

## 12G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12g/a">a</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/a/solution">Solution</h4>

↑ **Parent:** [A](#12g/a)

The [Laurent theorem](../../../analysis.md#laurent-theorem) says that if $f$ is analytic on an annulus

$$
r<|z-a|<R,
$$

then it has a unique [Laurent series](../../../analysis.md#laurent-series)

$$
f(z)=\sum_{n=-\infty}^{\infty}c_n(z-a)^n
$$

converging locally uniformly on that annulus, where

$$
c_n=\frac1{2\pi i}\oint_C\frac{f(\zeta)}{(\zeta-a)^{n+1}}\,d\zeta
$$

for any positively oriented circle $C$ in the annulus around $a$.

An [isolated singularity](../../../isolated-singularity.md) at $a$ is a point at which $f$ is not analytic although it is analytic on some punctured neighbourhood. It is removable when every $c_n$ with $n<0$ vanishes; it is a pole of order $m$ when $c_{-m}\ne0$ and $c_n=0$ for $n<-m$; and it is essential when infinitely many negative-index coefficients are nonzero.

For $0<|z|<1$,

$$
\frac1{z(z-1)}
=-\frac1z\frac1{1-z}
=-\sum_{n=0}^{\infty}z^{n-1}.
$$

For $|z|>1$,

$$
\frac1{z(z-1)}
=\frac1{z^2}\frac1{1-z^{-1}}
=\sum_{n=0}^{\infty}z^{-n-2}.
$$

The coefficients are unique after the annulus is fixed; these expansions differ because they represent the function on different annuli. At zero the first expansion has principal part $-z^{-1}$, so zero is a simple pole with residue $-1$.

<h3 id="12g/b">b</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/b/solution">Solution</h4>

↑ **Parent:** [B](#12g/b)

Put $g=1/f$. The hypothesis $|f(z)|\to\infty$ gives $g(z)\to0$ as $z\to a$, so defining $g(a)=0$ makes $g$ continuous on $U$ and analytic there by the stated assumption. Its zero at $a$ has some finite order $m\geq1$, and hence

$$
g(z)=(z-a)^m q(z),
\qquad q(a)\ne0.
$$

Therefore

$$
f(z)=(z-a)^{-m}\frac1{q(z)}
$$

has a pole of order $m$: its Laurent series has $c_{-m}\ne0$ and $c_n=0$ for $n<-m$.

Now let $f$ be entire and tend to infinity at infinity. The function

$$
h(z)=f(1/z)
$$

tends to infinity as $z\to0$, so the preceding argument says that $h$ has a pole at zero. If the [Taylor series](../../../calculus.md#taylor-series) of $f$ is $f(w)=\sum_{n\geq0}a_nw^n$, then

$$
h(z)=\sum_{n\geq0}a_nz^{-n}.
$$

A pole has only finitely many negative powers, so $a_n=0$ for all sufficiently large $n$. Thus $f$ is a [polynomial](../../../polynomial.md).

<h3 id="12g/c">c</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/c/solution">Solution</h4>

↑ **Parent:** [C](#12g/c)

For

$$
g(z)=\frac{e^z-1}{z\log(1+z)},
$$

both $e^z-1$ and $\log(1+z)$ have a simple zero at zero. Hence $g$ has a simple pole, and its [residue](../../../analysis.md#residue) is

$$
\operatorname{Res}(g,0)
=\lim_{z\to0}\frac{e^z-1}{\log(1+z)}
=\boxed{1}.
$$

For $h(z)=\sin z\sin(1/z)$, multiplication of the two Laurent series shows that all powers are even:

$$
h(z)=
\sum_{p,q\geq0}
\frac{(-1)^{p+q}}{(2p+1)!(2q+1)!}\,
z^{2(p-q)}.
$$

There are infinitely many negative powers, so zero is an [essential singularity](../../../isolated-singularity.md#essential-singularity). There is no $z^{-1}$ term, and therefore

$$
\boxed{\operatorname{Res}(h,0)=0}.
$$

## 13C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13c/a">a</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/a/solution">Solution</h4>

↑ **Parent:** [A](#13c/a)

With $\xi=x+ct$ and $\eta=x-ct$,

$$
\partial_x=\partial_\xi+\partial_\eta,
\qquad
\partial_t=c\partial_\xi-c\partial_\eta,
$$

so the [wave equation](../../../wave-equation.md) becomes

$$
u_{tt}-c^2u_{xx}=-4c^2u_{\xi\eta}=0.
$$

Thus $u=F(\xi)+G(\eta)$. At $t=0$ the initial data give

$$
F(x)+G(x)=\phi(x),
\qquad
cF'(x)-cG'(x)=\psi(x).
$$

Solving for $F'$ and $G'$ and integrating gives [d'Alembert's formula](../../../wave-equation.md#d-alembert-s-formula)\>

$$
\boxed{
u(x,t)=\frac{\phi(x+ct)+\phi(x-ct)}2
+\frac1{2c}\int_{x-ct}^{x+ct}\psi(s)\,ds }.
$$

<h3 id="13c/b">b</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/b/solution">Solution</h4>

↑ **Parent:** [B](#13c/b)

Extend the forcing oddly across the boundary:

$$
f_{\rm odd}(y,s)=
\begin{cases}
f(y,s),&y\geq0,\\
-f(-y,s),&y<0.
\end{cases}
$$

The initial displacement $\sin x$ is already odd, so its homogeneous evolution on the line is $\sin x\cos(ct)$. Applying [Duhamel's principle](../../../diffusion-equation.md#duhamel-s-principle) to the odd extension gives

$$
\boxed{
u(x,t)=\sin x\cos(ct)
+\frac1{2c}\int_0^t
\int_{x-c(t-s)}^{x+c(t-s)}
f_{\rm odd}(y,s)\,dy\,ds }.
$$

The odd-reflection method makes $u(0,t)=0$. At $t=0$ the double integral vanishes together with its first time derivative, so the prescribed initial displacement and velocity are also satisfied.

## 14C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14c/i">i</h3>

↑ **Parent:** [14C](#14c)

<h4 id="14c/i/solution">Solution</h4>

↑ **Parent:** [I](#14c/i)

For a normalized wavefunction obeying the infinite-wall [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition), integration by parts gives the energy expectation

$$
\langle H\rangle
=\int_0^a\left(\frac{\hbar^2}{2m}|\psi'(x)|^2
+U(x)|\psi(x)|^2\right)\,dx\geq0.
$$

Thus every [energy eigenvalue](../../../quantum-mechanics.md#energy-eigenvalue) is nonnegative.

For $0<E<U_0$, the [Time-independent Schrödinger equation](../../../physics.md#time-independent-schrodinger-equation) and the wall conditions give

$$
\psi(x)=
\begin{cases}
A\sin(kx),&0\leq x\leq a/2,\\
B\sinh(l(a-x)),&a/2\leq x\leq a,
\end{cases}
$$

where $k=\sqrt{2mE}/\hbar$ and $l=\sqrt{2m(U_0-E)}/\hbar$. Continuity of $\psi$ and $\psi'$ at the finite potential step gives

$$
A\sin(ka/2)=B\sinh(la/2),
$$



$$
Ak\cos(ka/2)=-Bl\cosh(la/2).
$$

Dividing and rearranging yields the [bound-state quantization condition](../../../physics.md#bound-state-quantization-condition)

$$
\boxed{\frac1k\tan\frac{ka}{2}
=-\frac1l\tanh\frac{la}{2}}.
$$

<h3 id="14c/ii">ii</h3>

↑ **Parent:** [14C](#14c)

<h4 id="14c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#14c/ii)

Before the change, the normalized [ground state](../../../quantum-mechanics.md#ground-state) of the infinite square well is

$$
\psi_0(x)=\sqrt{\frac2a}\sin\frac{\pi x}{a}.
$$

For an allowed post-quench energy $E\in(0,U_0)$ satisfying part (i), define the unnormalized eigenfunction

$$
\chi_E(x)=
\begin{cases}
\sin(kx),&0\leq x\leq a/2,\\[2pt]
\dfrac{\sin(ka/2)}{\sinh(la/2)}
\sinh(l(a-x)),&a/2\leq x\leq a.
\end{cases}
$$

Its normalization factor is

$$
N_E^{-2}=
\int_0^{a/2}\sin^2(kx)\,dx
+\frac{\sin^2(ka/2)}{\sinh^2(la/2)}
\int_{a/2}^{a}\sinh^2(l(a-x))\,dx.
$$

The [Born rule](../../../quantum-mechanics.md#born-rule) therefore gives

$$
\boxed{
\operatorname{prob}(E)
=\frac{2N_E^2}{a}
\left|
\int_0^{a/2}\sin\frac{\pi x}{a}\sin(kx)\,dx
+\frac{\sin(ka/2)}{\sinh(la/2)}
\int_{a/2}^{a}\sin\frac{\pi x}{a}\sinh(l(a-x))\,dx
\right|^2 }.
$$

For a value of $E$ that is not an eigenvalue, this probability is zero. The sudden change leaves the wavefunction fixed, while the energy eigenbasis changes.

## 15D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

Since the [magnetic field](../../../electromagnetism.md#magnetic-field) is $B=\nabla\times A$, [Stokes theorem](../../../calculus.md#stokes-theorem) gives, for any oriented surface $S$ bounded by $C$,

$$
\Phi=\int_SB\mathbin{\cdot}dS
=\int_S(\nabla\times A)\mathbin{\cdot}dS
=\boxed{\oint_CA\mathbin{\cdot}dx}.
$$

Under a [gauge transformation](../../../electromagnetism.md#gauge-transformation) $A\mapsto A+\nabla\chi$, the integral changes by

$$
\oint_C\nabla\chi\mathbin{\cdot}dx=0
$$

because $C$ is closed. The flux expression is therefore gauge independent.

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/solution">Solution</h4>

↑ **Parent:** [B](#15d/b)

The magnetostatic [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) is $\nabla\times B=\mu_0J$. Substituting $B=\nabla\times A$ and using the [Coulomb gauge](../../../electromagnetism.md#coulomb-gauge) $\nabla\mathbin{\cdot}A=0$ gives

$$
\mu_0J=\nabla\times(\nabla\times A)
=\nabla(\nabla\mathbin{\cdot}A)-\nabla^2A
=-\nabla^2A.
$$

The free-space [Green function of the Laplacian](../../../partial-differential-equation.md#green-function-of-the-laplacian) therefore gives

$$
A(x)=\frac{\mu_0}{4\pi}
\int_{\mathbb R^3}\frac{J(x')}{|x-x'|}\,d^3x'.
$$

For the thin wire current stated in the question this becomes

$$
\boxed{
A(x)=\frac{\mu_0I}{4\pi}\oint_C\frac{dx'}{|x-x'|}}.
$$

<h3 id="15d/c">c</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/c/solution">Solution</h4>

↑ **Parent:** [C](#15d/c)

Substituting the wire potential from part (b) into the flux formula from part (a) gives [Neumann's mutual-inductance formula](../../../electromagnetism.md#neumann-s-mutual-inductance-formula)

$$
L_{12}
=\frac{\Phi_{12}}{I_2}
=\frac{\mu_0}{4\pi}
\oint_{C_1}\oint_{C_2}
\frac{dx_1\mathbin{\cdot}dx_2}{|x_1-x_2|}.
$$

Interchanging the two curves proves $L_{12}=L_{21}$.

Parametrize the coaxial circles by

$$
x_1=(a\cos\phi,a\sin\phi,0),
\qquad
x_2=(b\cos\psi,b\sin\psi,c).
$$

Then, with $\theta=\phi-\psi$ and $R=\sqrt{a^2+b^2+c^2}$,

$$
dx_1\mathbin{\cdot}dx_2
=ab\cos\theta\,d\phi\,d\psi,
\qquad
|x_1-x_2|=R\sqrt{1-q\cos\theta},
$$

where $q=2ab/R^2$. One angular integration contributes $2\pi$, so

$$
L_{12}
=\frac{\mu_0ab}{2R}
\int_0^{2\pi}\frac{\cos\theta\,d\theta}
{\sqrt{1-q\cos\theta}}.
$$

Since $ab=qR^2/2$, this is

$$
\boxed{
L_{12}=\frac{\mu_0R}{4}f(q)
=\frac{\mu_0}{4}\sqrt{a^2+b^2+c^2}\,f(q)}.
$$

## 16A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16a/a">a</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/a/solution">Solution</h4>

↑ **Parent:** [A](#16a/a)

For a [velocity potential](../../../fluid-mechanics.md#velocity-potential), $u=\nabla\phi$. Writing $\theta=x-t$ gives

$$
\boxed{u=(\varepsilon y\cos\theta,\varepsilon\sin\theta)}.
$$

Its [divergence](../../../calculus.md#divergence) is

$$
\boxed{\nabla\mathbin{\cdot}u
=-\varepsilon y\sin\theta}.
$$

**Thus this potential flow is generally compressible.**

<h3 id="16a/b">b</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/b/solution">Solution</h4>

↑ **Parent:** [B](#16a/b)

Both $\sin(x-t)$ and $\cos(x-t)$ have zero average over one period, so $\langle u\rangle=0$ at every fixed point.

The [material derivative](../../../continuum-mechanics.md#material-derivative) gives the particle acceleration

$$
a=\frac{\partial u}{\partial t}+(u\mathbin{\cdot}\nabla)u.
$$

Direct differentiation yields

$$
a_x=\varepsilon y\sin\theta
+\varepsilon^2(1-y^2)\sin\theta\cos\theta,
$$



$$
a_y=-\varepsilon\cos\theta
+\varepsilon^2y\cos^2\theta.
$$

Therefore the [Eulerian time average](../../../continuum-mechanics.md#eulerian-time-average) at fixed $(x,y)$ is

$$
\boxed{\langle a\rangle=(0,\varepsilon^2y/2)}.
$$

<h3 id="16a/c">c</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/c/solution">Solution</h4>

↑ **Parent:** [C](#16a/c)

The dyed particle satisfies the [Lagrangian trajectory](../../../continuum-mechanics.md#lagrangian-trajectory) equations

$$
\dot x=\varepsilon y\cos(x-t),
\qquad
\dot y=\varepsilon\sin(x-t),
\qquad
x(0)=y(0)=0.
$$

For the proposed approximation, $x=O(\varepsilon^2)$ and

$$
\dot y=-\varepsilon\sin t
=\varepsilon\sin(x-t)+O(\varepsilon^3).
$$

Also

$$
\dot x
=\varepsilon^2(\cos^2t-\cos t)
=\varepsilon y\cos(x-t)+O(\varepsilon^3).
$$

The initial conditions hold, verifying

$$
x=\varepsilon^2\left(\frac14\sin2t+\frac t2-\sin t\right),
\qquad
y=\varepsilon(\cos t-1)
$$

through order $\varepsilon^2$.

Over one period, the periodic terms return to their initial values while the secular term changes $x$ by $\varepsilon^2\pi$. Hence the dyed particle has [Stokes drift](../../../continuum-mechanics.md#stokes-drift)

$$
\boxed{\overline v_{\rm particle}
=\left(\frac{\varepsilon^2}{2},0\right)}
$$

to this order, despite the zero Eulerian mean velocity.

## 17B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17b/i">i</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/i/solution">Solution</h4>

↑ **Parent:** [I](#17b/i)

The [local truncation error](../../../numerical-analysis.md#local-truncation-error) is the error made by one numerical step started from the exact solution:

$$
\tau_{n+1}
=y(t_{n+1})-y(t_n)
-h\phi(t_n,y(t_n),h).
$$

A one-step method has local order $p+1$ when $\tau_{n+1}=O(h^{p+1})$ uniformly for $t_n$ in each fixed bounded time interval.

<h3 id="17b/ii">ii</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#17b/ii)

Let $e_n=y^n-y(t_n)$. Subtracting the exact one-step relation from the numerical method and applying the stated [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) gives

$$
\|e_{n+1}\|
\leq(1+hL)\|e_n\|+\|\tau_{n+1}\|.
$$

If $\|\tau_{n+1}\|\leq Ch^{p+1}$, iteration yields the [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality)

$$
\|e_n\|
\leq(1+hL)^n\|e_0\|
+Ch^{p+1}\sum_{j=0}^{n-1}(1+hL)^j.
$$

For $nh\leq t^*$,

$$
(1+hL)^n\leq e^{nhL}\leq e^{t^*L}
$$

and

$$
h^{p+1}\sum_{j=0}^{n-1}(1+hL)^j
\leq\frac{e^{t^*L}-1}{L}h^p.
$$

Consequently

$$
\boxed{
\max_{0\leq n\leq\lfloor t^*/h\rfloor}
\|y^n-y(nh)\|
\leq e^{t^*L}\|e_0\|+O(h^p)}.
$$

<h3 id="17b/iii">iii</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#17b/iii)

Here

$$
\phi(u,h)=\frac14\left[
f(u)+3f\left(u+\frac{2h}{3}f(u)\right)\right].
$$

For $0<h\leq1$, the Lipschitz bound on $f$ gives

$$
|\phi(u,h)-\phi(v,h)|
\leq\left(K+\frac{K^2}{2}\right)|u-v|,
$$

so part (ii) applies with a constant independent of sufficiently small $h$.

The exact solution has the [Taylor expansion](../../../calculus.md#taylor-series)\>

$$
y(t+h)=y(t)+hf(y(t))
+\frac{h^2}{2}f'(y(t))f(y(t))+O(h^3).
$$

Meanwhile,

$$
f\left(y+\frac{2h}{3}f(y)\right)
=f(y)+\frac{2h}{3}f'(y)f(y)+O(h^2),
$$

so one numerical step from $y$ is

$$
y+h\phi(y,h)
=y+hf(y)+\frac{h^2}{2}f'(y)f(y)+O(h^3).
$$

The local error is therefore $O(h^3)$. Taking $p=2$ in part (ii) proves the required second-order global-error bound. This method is a two-stage [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method).

## 18H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

The [moment-generating function](../../../probability-theory.md#moment-generating-function) of $W_i\sim\operatorname{Exp}(1)$ is

$$
M_{W_i}(t)=\frac1{1-t},
\qquad t<1.
$$

Independence makes the moment-generating function of the sum equal the product:

$$
M_{\sum_iW_i}(t)=(1-t)^{-n}.
$$

This is the moment-generating function of the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) $\Gamma(n,1)$, and moment-generating functions determine distributions in a neighbourhood of zero. Hence

$$
\boxed{\sum_{i=1}^nW_i\sim\Gamma(n,1)}.
$$

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

For $y\geq0$ and $X\sim U(0,1)$,

$$
\Pr(-\log X\leq y)
=\Pr(X\geq e^{-y})
=1-e^{-y}.
$$

The distribution function is zero for $y<0$, so this is exactly the distribution function of $\operatorname{Exp}(1)$. Therefore

$$
\boxed{-\log X\sim\operatorname{Exp}(1)}.
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) states that, for testing one simple hypothesis with density $f_0$ against another with density $f_1$, a size-$\alpha$ test that rejects for the largest values of the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) $f_1/f_0$ is most powerful among all tests of size at most $\alpha$, with boundary randomization if needed.

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

The normalized density is

$$
f_\theta(x)=(\theta+1)x^\theta\mathbf1_{(0,1)}(x).
$$

For $\theta=1$ against $\theta=0$, the sample likelihood ratio is

$$
\frac{L(1)}{L(0)}
=2^n\prod_{i=1}^nX_i
=2^ne^{-S},
\qquad
S=-\sum_{i=1}^n\log X_i.
$$

It is strictly decreasing in $S$. Under $H_0$, parts (a) and (b) give

$$
S\sim\Gamma(n,1).
$$

If $q_\alpha$ is the lower $\alpha$-quantile of this gamma distribution, the [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) gives the most powerful size-$\alpha$ critical region

$$
\boxed{S\leq q_\alpha}.
$$

For any fixed $\theta>0$,

$$
\frac{L(\theta)}{L(0)}
=(\theta+1)^ne^{-\theta S}
$$

is again strictly decreasing in the same statistic $S$. Thus the same critical region is most powerful against every $\theta>0$ and is consequently a [uniformly most powerful test](../../../statistical-modelling.md#uniformly-most-powerful-test) of $H_0:\theta=0$ against $H_1:\theta>0$.

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

A random time $T$ is a [stopping time](../../../martingale.md#stopping-time) when the event $\{T\leq n\}$ is determined by $X_0,\ldots,X_n$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) says that, conditionally on $T<\infty$ and $X_T=x$, the process $(X_{T+k})_{k\geq0}$ is a fresh Markov chain started at $x$, independent of the history before $T$.

Use the state space $\{1,2,4\}\times\mathbb Z_{\geq0}$, with $(2,0)$ absorbing. Observe the chain only when it is at square 2. From $(2,k)$, the change $Y$ in wealth by the next return to square 2 has distribution

$$
\Pr(Y=-1)=\frac12,\qquad
\Pr(Y=1)=\frac18,\qquad
\Pr(Y=2)=\frac38.
$$

Indeed, heads lands on square 3 and returns to square 2 after losing £1. After tails reaches square 4, the remaining two or three moves give the other cases.

For $r=2/3$,

$$
\mathbb E[r^Y]
=\frac12r^{-1}+\frac18r+\frac38r^2=1.
$$

Thus $r^{M_j}$ is a [martingale](../../../martingale.md) for the embedded wealth random walk $M_j$. Stopping when it first reaches $m-1$ or a large upper level and then letting that level tend to infinity gives

$$
\Pr_{(2,m)}(\text{ever hit }(2,m-1))=r=\boxed{\frac23}.
$$

The upper-bound contribution vanishes because $0<r<1$; equivalently, this is the smaller probability solution of the first-step equation.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

By part (a) and repeated use of the [Strong Markov property](../../../markov-process.md#strong-markov-property), the probability of descending from $(2,k)$ to $(2,0)$ is

$$
\left(\frac23\right)^k.
$$

Starting from square 1 with £$m$, heads moves to $(2,m)$, whereas tails lands on square 3, loses £1, and moves to $(2,m-1)$. Therefore the loss probability is

$$
\frac12\left(\frac23\right)^m
+\frac12\left(\frac23\right)^{m-1}
=\boxed{\frac56\left(\frac23\right)^{m-1}}.
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
