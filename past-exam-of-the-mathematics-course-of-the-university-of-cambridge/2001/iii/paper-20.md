# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper20.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We first give an auxiliary-integral proof, rather than deducing both requested results from a theorem only stated later. The following [symmetric Hermite integral obstruction](../../../number-theory.md#symmetric-hermite-integral-obstruction) will do both jobs. Suppose

$$
k+\sum_{j=1}^s b_je^{\beta_j}=0,
$$

where $k\ne0$ and $b_j$ are [integers](../../../number-theory.md#integer), the distinct nonzero algebraic exponents form a Galois-stable set, and their weights are invariant under conjugation. Choose $P\in\mathbb Z[X]$ vanishing at those exponents, with $P(0)\ne0$, and a positive [integer](../../../number-theory.md#integer) $c$ for which every $c\beta_j$ is an [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer). For a large [prime number](../../../number-theory.md#prime-number) $p$, let

$$
D=(\deg P+1)p-1,\qquad f_p(X)=\frac{c^DX^{p-1}P(X)^p}{(p-1)!},\qquad F_p(X)=\sum_{r=0}^D f_p^{(r)}(X).
$$

At zero, derivatives below $p-1$ vanish; the derivative of order $p-1$ equals $c^DP(0)^p$. All higher derivatives at zero are [integers](../../../number-theory.md#integer) divisible by $p$. At each $\beta_j$, derivatives below $p$ vanish and all higher derivatives belong to $p\mathcal O_L$ in a Galois [splitting field](../../../galois-theory.md#splitting-field) $L$. Indeed their coefficients contain $r!/(p-1)!$, divisible by $p$ for $r\ge p$, and every $c^D\beta_j^u$ is integral for $u\le D$. Consequently

$$
I_p=kF_p(0)+\sum_jb_jF_p(\beta_j)\in\mathbb Z,\qquad I_p\equiv kc^DP(0)^p\pmod p.
$$

Galois invariance makes the sum rational, and integrality makes it an [integer](../../../number-theory.md#integer). For [prime numbers](../../../number-theory.md#prime-number) not dividing $kcP(0)$ it is nonzero.

But $F_p-F_p'=f_p$, so integration along the straight segment to $\beta$ gives

$$
e^\beta F_p(0)-F_p(\beta)=\int_0^\beta e^{\beta-z}f_p(z)\,dz.
$$

Multiply by the weights and use the assumed exponential relation. This expresses $-I_p$ as the sum of these integrals. On the finitely many fixed segments, their absolute values are at most $C^p/(p-1)!$ for a fixed $C$: all [polynomial](../../../polynomial.md) and exponential factors have fixed bounds, and $D$ is linear in $p$. Thus $|I_p|\to0$, contradicting its being a nonzero [integer](../../../number-theory.md#integer). The obstruction is proved.

If $e$ were algebraic, an integral [polynomial](../../../polynomial.md) relation would give $a_0+\sum_{j=1}^s a_je^j=0$ with $a_0\ne0$. [Integer](../../../number-theory.md#integer) exponents and weights satisfy the obstruction, so **$e$ is transcendental**.

If $\pi$ were algebraic, put $\alpha=i\pi$ and let $\alpha_1,\ldots,\alpha_d$ be its algebraic conjugates. Since $1+e^\alpha=0$, the product $\prod_j(1+e^{\alpha_j})$ vanishes. Expand it and collect equal subset sums. The zero sums contribute a positive [integer](../../../number-theory.md#integer) $k\ge1$; the nonzero sums give a Galois-stable list $\beta_j$ with positive integral multiplicities. This is precisely the prohibited relation. Hence **$\pi$ is transcendental**.

The general [Lindemann–Weierstrass theorem](../../../number-theory.md#lindemann-weierstrass-theorem) states that exponentials of distinct [algebraic numbers](../../../algebra.md#algebraic-number) are linearly independent over $\overline{\mathbb Q}$. Suppose the sine quotient were algebraic, say $\gamma$. The denominator is nonzero: $\sin\beta=0$ would give a forbidden relation between the exponentials of the distinct [algebraic numbers](../../../algebra.md#algebraic-number) $i\beta,-i\beta$. The quotient identity would give

$$
e^{i\alpha}-e^{-i\alpha}-\gamma e^{i\beta}+\gamma e^{-i\beta}=0.
$$

The four exponents are distinct under the stated nonzero and non-opposite assumptions, so this also contradicts [linear independence](../../../vector-space.md#linear-independence). Therefore

$$
\boxed{\sin\alpha/\sin\beta\text{ is transcendental}}.
$$

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

We prove the Mahler alternative in full. Let $f(z)=\sum_{n\ge0}z^{l^n}$. Its series converges locally uniformly in the [unit disc](../../../topology.md#unit-disc) and satisfies

$$
f(z^l)=f(z)-z.
$$

It is transcendental as a function. At a [root of unity](../../../algebra.md#root-of-unity) $\zeta$ with $\zeta^{l^r}=1$, the radial tail $\sum_{n\ge r}t^{l^n}$ in $f(t\zeta)$ is real and tends to infinity as $t\uparrow1$, while the initial terms remain bounded. These roots are dense on the [unit](../../../algebra.md#unit-in-a-ring) circle. An algebraic function can have singularities only at the finitely many zeros of its leading coefficient and [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant): elsewhere its defining [polynomial](../../../polynomial.md) and the implicit-function theorem give local analytic branches. Hence $f$ cannot be algebraic over $\mathbb C(z)$.

Assume now that $\alpha$ and $f(\alpha)$ are algebraic, with $0<|\alpha|<1$, and put both in a [number field](../../../algebraic-number-theory.md#number-field) $K$ of degree $d$. For each $N$, the $(N+1)^2$ coefficients of a [polynomial](../../../polynomial.md) $P_N(X,Y)$ of bidegree at most $N$ can cancel the first $(N+1)^2-1$ Taylor coefficients of $P_N(z,f(z))$. The equations have [integer](../../../number-theory.md#integer) coefficients, so a nonzero [integer](../../../number-theory.md#integer) solution exists after clearing denominators. Functional transcendence makes $R_N(z)=P_N(z,f(z))$ nonzero. Its order $T_N$ at zero satisfies $T_N\ge(N+1)^2-1$.

At $\alpha_r=\alpha^{l^r}$ the [functional equation](../../../analysis.md#functional-equation) gives $f(\alpha_r)=f(\alpha)-\sum_{j<r}\alpha^{l^j}\in K$. Thus $\eta_r=R_N(\alpha_r)\in K$ is nonzero for all sufficiently large $r$ and

$$
\log|\eta_r|\le-T_Nl^r\log(1/|\alpha|)+O_N(1).
$$

Use the absolute [logarithmic height](../../../algebraic-number-theory.md#absolute-logarithmic-weil-height) $h$. The elementary inequalities for sums and [polynomial](../../../polynomial.md) evaluation give

$$
h(\eta_r)\le N\left(1+\frac1{l-1}\right)l^rh(\alpha)+O_N(r+1).
$$

Here $h(f(\alpha_r))\le h(f(\alpha))+(l^r-1)h(\alpha)/(l-1)+r\log2$. The [Liouville height inequality](../../../algebraic-number-theory.md#liouville-height-inequality) gives $\log|\eta_r|\ge-dh(\eta_r)$. Divide by $l^r$ and let $r\to\infty$ to obtain

$$
T_N\log(1/|\alpha|)\le dN\frac l{l-1}h(\alpha).
$$

The left grows quadratically in $N$, the right only linearly. Choose $N$ large to contradict this. Hence **every such algebraic $\alpha$ has transcendental $f(\alpha)$**. This is the [auxiliary-value height argument for the Fredholm series](../../../number-theory.md#auxiliary-value-height-argument-for-the-fredholm-series).

For the rational continuation, let $a_n=\sum_{j=0}^n(p/q)^{l^j}$ and $Q_n=q^{l^n}$. This is a [rational number](../../../number-theory.md#rational-number) with reduced denominator $B_n\le Q_n$, and its positive tail satisfies, for large $n$,

$$
0<f(p/q)-a_n\le2(p/q)^{l^{n+1}}=2Q_n^{-\kappa},\qquad\kappa=l\left(1-\frac{\log p}{\log q}\right)>l(1-\delta)>2.
$$

A rational value $a/b$ would instead have distance at least $1/(bQ_n)$ from each distinct $a_n$, already impossible. If the value were algebraic irrational, choose $\epsilon>0$ with $2+\epsilon<\kappa$. The distinct truncations have unbounded reduced denominators, and the displayed errors are eventually smaller than $B_n^{-2-\epsilon}$. This contradicts [Roth theorem](../../../number-theory.md#roth-s-theorem). Thus the requested rational values are transcendental by the [Roth criterion for rational Fredholm values](../../../number-theory.md#roth-criterion-for-rational-fredholm-values).

For completeness, the elliptic alternative's conclusion also has a short auxiliary-divisor certificate. If $\Phi$ is Frobenius on $E/\mathbb F_q$, then $\deg\Phi=q$ and $\deg(1-\Phi)=N=\#E(\mathbb F_q)$: the latter map is separable and its kernel is exactly the rational points. The [divisor](../../../number-theory.md#divisor) identity for $x(P)-x(Q)$ on $E\times E$ gives the parallelogram rule $\deg(u+v)+\deg(u-v)=2\deg u+2\deg v$. Polarizing it yields

$$
\deg(m+n\Phi)=m^2+tmn+qn^2,\qquad t=q+1-N.
$$

All these degrees are nonnegative. In particular $\deg(-t+2\Phi)=4q-t^2\ge0$, so $|t|\le2\sqrt q$. The Frobenius characteristic [polynomial](../../../polynomial.md) is $X^2-tX+q$; its complex roots have modulus $\sqrt q$, including the double-root case. The zeta function has numerator $1-tT+qT^2$, whose zeros consequently have modulus $q^{-1/2}$, the elliptic Riemann hypothesis. This supplements the fully proved Mahler branch with the [degree-form proof of the Hasse bound](../../../normalization-of-an-algebraic-curve.md#degree-form-proof-of-the-hasse-bound); it is an auxiliary-divisor proof, not a claim that an unspecified transcendence theorem proves the bound.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Gelfond–Schneider theorem](../../../number-theory.md#gelfond-schneider-theorem) says that if $a\ne0,1$ is algebraic and $\beta$ is algebraic irrational, then every value $\exp(\beta\lambda)$ with $e^\lambda=a$ is transcendental. Fix such a nonzero logarithm $\lambda$, and suppose $\gamma=e^{\beta\lambda}$ is algebraic. The [field](../../../algebra.md#field) $K=\mathbb Q(a,\beta,\gamma)$ then contains all values needed in [Schneider lattice proof of the Gelfond–Schneider theorem](../../../number-theory.md#schneider-lattice-proof-of-the-gelfond-schneider-theorem).

Here is an outline including the parameter balance. For a large $L$, choose [polynomial](../../../polynomial.md) degrees $M\asymp L\log L$, $N\asymp L/\log L$, with constants large enough that $(M+1)(N+1)>[K:\mathbb Q]L^2$. Impose

$$
P(s+t\beta,a^s\gamma^t)=0\qquad(0\le s,t<L).
$$

Expand these $K$-linear equations in a rational basis and clear denominators. [Siegel lemma](../../../number-theory.md#siegel-s-lemma) gives a nonzero [integer](../../../number-theory.md#integer) [polynomial](../../../polynomial.md) $P$ with $\log H(P)=O(L^2/\log L)$. This follows because each coefficient in the grid equations has [arithmetic height](../../../algebraic-number-theory.md#height-function) $O(M\log L+NL)$ and the ratio of unknowns to constraints stays bounded away from one. The [exponential polynomial](../../../complex-analysis.md#exponential-polynomial) $F(z)=P(z,e^{\lambda z})$ is not identically zero: distinct exponentials are independent over the [polynomial](../../../polynomial.md) ring, as one sees by successively applying powers of $D-j\lambda$ to kill all but one term.

The irrationality of $\beta$ makes the $L^2$ grid points distinct. Their zeros make subsequent grid values extremely small. More precisely, if a whole $S\times S$ grid has been obtained, take an outer radius $R\asymp S\log S$. Growth gives $\log\max_{|z|=R}|F(z)|\le\log H(P)+O(M\log R+NR)$. The product form of Schwarz's lemma contributes $(C/\log S)^{S^2}$ at the next grid points. Therefore

$$
\log|F(s+t\beta)|\le-cS^2\log\log S\qquad(s,t\le S)
$$

for large initial $L$, unless the value is zero. But every such value is algebraic in the same $K$, since $e^{\lambda(s+t\beta)}=a^s\gamma^t$. Its [arithmetic height](../../../algebraic-number-theory.md#height-function) is $O(\log H(P)+M\log S+NS)$, so the Liouville lower bound is incompatible with the displayed upper bound for a nonzero value. Induction extends the zero grid indefinitely.

A fixed nonzero [exponential polynomial](../../../complex-analysis.md#exponential-polynomial) has only $O(R)$ zeros in a disc of radius $R$, by its exponential-type growth and [Jensen's formula](../../../complex-analysis.md#jensen-s-formula) centered at a nonzero value. The grids give $S^2$ distinct zeros in a disc of radius $O(S)$, a contradiction. Thus **$a^\beta$ is transcendental for every choice of logarithm**, completing the [Schneider lattice proof of the Gelfond–Schneider theorem](../../../number-theory.md#schneider-lattice-proof-of-the-gelfond-schneider-theorem).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

A standard form of the [Schneider-Lang theorem](../../../number-theory.md#schneider-lang-theorem) is this. Let $f_1,\ldots,f_s$ be meromorphic functions with $f_j'\in K[f_1,\ldots,f_s]$ for a fixed [number field](../../../algebraic-number-theory.md#number-field) $K$. Suppose $f_1,f_2$ have [algebraic independence](../../../algebra.md#algebraic-independence) over $\mathbb C$ and have finite growth orders $\rho_1,\rho_2$. There are at most $[K:\mathbb Q](\rho_1+\rho_2)$ points at which all the functions are finite and all their values lie in $K$.

Take $f_1(z)=z$ and $f_2(z)=e^z$, of orders zero and one. Their derivatives belong to $K[z,e^z]$. They have [algebraic independence](../../../algebra.md#algebraic-independence): a [polynomial](../../../polynomial.md) relation $\sum_jp_j(z)e^{jz}=0$ is impossible by exponential-polynomial independence, or by letting real $z$ tend to infinity and considering the largest $j$.

If nonzero algebraic $\alpha$ had algebraic $e^\alpha$, put $K=\mathbb Q(\alpha,e^\alpha)$. At each of the distinct points $z=n\alpha$, both $z$ and $e^z=(e^\alpha)^n$ belong to $K$. Infinitely many points contradict the theorem's finite bound. Therefore

$$
\boxed{e^\alpha\text{ is transcendental whenever }0\ne\alpha\in\overline{\mathbb Q}}.
$$

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For $M<N$ homogeneous equations $\sum_{j=1}^N a_{ij}z_j=0$ with integral coefficients $|a_{ij}|\le A$, $A\ge1$, [Siegel lemma](../../../number-theory.md#siegel-s-lemma) supplies a nonzero integral vector with

$$
0<\|z\|_\infty\le Q=\left\lfloor(2NA)^{M/(N-M)}\right\rfloor.
$$

Map the [integer](../../../number-theory.md#integer) box $\{0,\ldots,Q\}^N$ to the $M$ equation values. There are $(Q+1)^N$ inputs, while each output coordinate lies in $[-NAQ,NAQ]$, so there are at most $(2NAQ+1)^M$ outputs. Since $Q+1>(2NA)^{M/(N-M)}$ and $2NAQ+1\le2NA(Q+1)$, the input count is strictly larger. Two inputs have the same image; their nonzero difference solves every equation and has the stated norm bound. This proves the lemma by the [pigeonhole proof of integer Siegel lemma](../../../number-theory.md#pigeonhole-proof-of-integer-siegel-lemma).

Rational coefficients are handled by clearing denominators. For coefficients in a [number field](../../../algebraic-number-theory.md#number-field) of degree $d$, expansion in a rational basis gives at most $dM$ rational equations; if $N>dM$ the same argument gives an [integer](../../../number-theory.md#integer) solution with the corresponding effective bound after clearing the basis denominators. The lemma concerns homogeneous equations; arbitrary inhomogeneous [integer](../../../number-theory.md#integer) equations need not be soluble.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

In Siegel's original convention, an [E-function](../../../number-theory.md#e-function) is an entire series $F(z)=\sum_{n\ge0}a_nz^n/n!$ with coefficients in a fixed [number field](../../../algebraic-number-theory.md#number-field), satisfying a nonzero [linear differential equation](../../../differential-equation.md#linear-differential-equation) over $\overline{\mathbb Q}(z)$, together with these arithmetic bounds: for every $\epsilon>0$, all conjugates of $a_0,\ldots,a_n$ have size $O_\epsilon(n^{\epsilon n})$, and some positive [integer](../../../number-theory.md#integer) $d_n=O_\epsilon(n^{\epsilon n})$ makes every $d_na_j$, $j\le n$, an [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer). A frequently used stricter convention replaces both bounds by $C^{n+1}$. The original and strict growth definitions should not simply be declared equivalent; the exponential examples below satisfy the strict one.

For sums, work in the [compositum](../../../algebra.md#field-compositum) of the coefficient fields. Coefficient conjugate bounds add. The product of the two common denominators clears both lists; using $\epsilon/2$ in each original denominator bound gives the required $O_\epsilon(n^{\epsilon n})$ product bound. Finally all derivatives of $F+G$ lie in the sum of the two finite-dimensional derivative spaces over that [rational function](../../../isolated-singularity.md#rational-function) [field](../../../algebra.md#field), so they satisfy a nontrivial [linear dependence](../../../vector-space.md#linear-dependence), giving a differential equation for the sum. Thus **sums are again E-functions**, the [addition closure of Siegel E-functions](../../../number-theory.md#addition-closure-of-siegel-e-functions).

The [Siegel–Shidlovsky theorem](../../../number-theory.md#siegel-shidlovsky-theorem) states that if a vector of E-functions satisfies $F'=A(z)F$ with rational-function matrix over $\overline{\mathbb Q}$, then at every nonzero algebraic $\xi$ which is not a pole of $A$,

$$
\operatorname{trdeg}_{\overline{\mathbb Q}}\overline{\mathbb Q}(F_1(\xi),\ldots,F_s(\xi))=\operatorname{trdeg}_{\overline{\mathbb Q}(z)}\overline{\mathbb Q}(z)(F_1(z),\ldots,F_s(z)).
$$

In particular algebraically independent functions give algebraically independent values.

Take $F_j(z)=e^{\gamma_jz}$ for [algebraic numbers](../../../algebra.md#algebraic-number) $\gamma_j$ linearly independent over $\mathbb Q$. Their coefficients are $\gamma_j^n$ with exponential conjugate and denominator bounds, and $F_j'=\gamma_jF_j$. A [polynomial](../../../polynomial.md) relation among the functions expands into a relation among exponentials with distinct exponents $\sum m_j\gamma_j$ and [polynomial](../../../polynomial.md) coefficients after clearing rational-function denominators; exponential-polynomial independence excludes it. At $\xi=1$ the theorem gives [algebraic independence](../../../algebra.md#algebraic-independence) of the $e^{\gamma_j}$. For arbitrary distinct algebraic $\alpha_i$, choose a rational basis of their span and divide that basis by a common denominator. The $e^{\alpha_i}$ are distinct Laurent monomials in the corresponding algebraically independent exponential values, so are linearly independent over $\overline{\mathbb Q}$. This recovers the general [Lindemann–Weierstrass theorem](../../../number-theory.md#lindemann-weierstrass-theorem). Its simplest instance uses just $F(z)=e^z$ at nonzero algebraic $\xi$.

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Fix [fundamental units](../../../algebraic-number-theory.md#fundamental-unit-number-theory) $\varepsilon_1,\ldots,\varepsilon_r$ and write $x=\zeta\prod\varepsilon_i^{b_i}$. Rank zero already gives a finite [unit group](../../../algebra.md#unit-group). Otherwise put $B=\max(1,|b_i|)$. The logarithmic embedding in Dirichlet's theorem has a weighted sum-zero image and is injective on the free exponent lattice. Norm equivalence and that sum-zero condition give an archimedean embedding $\sigma$ with

$$
|\sigma(x)|\le C e^{-cB}.
$$

This is the [small archimedean value of a large unit](../../../algebraic-number-theory.md#small-archimedean-value-of-a-large-unit). From the equation, $\sigma(\beta y)=1-\sigma(\alpha x)$ is exponentially close to one. Also $h(y)\le h(x)+O(1)$ by the [arithmetic height](../../../algebraic-number-theory.md#height-function) inequalities for $y=(1-\alpha x)/\beta$, so the fundamental-unit exponents of $y$ have size $O(B)$.

For large $B$, take the small-branch logarithm of $\sigma(\beta y)$. With $y=\eta\prod\varepsilon_i^{c_i}$ it is the nonzero form

$$
\Lambda=\log\sigma(\beta\eta)+\sum_i c_i\log\sigma(\varepsilon_i)-2k\log(-1),\qquad |k|=O(B),
$$

using fixed logarithms and $\log(-1)=\pi i$. The [integer](../../../number-theory.md#integer) $k$ corrects the branch, and nonzero follows since $\beta y=1$ would force $\alpha x=0$. Its upper bound is $|\Lambda|\le C'e^{-cB}$. The assumed effective logarithmic-form estimate for the fixed [algebraic numbers](../../../algebra.md#algebraic-number) gives $\log|\Lambda|\ge-C''\log(2B)$. Thus $cB\le C''\log(2B)+O(1)$, effectively bounding $B$. The finitely many embeddings and torsion choices give uniform constants. Therefore **there are only finitely many [unit](../../../algebra.md#unit-in-a-ring) solutions, and their exponents are effectively bounded**.

For the Thue application, take an irreducible integral [binary form](../../../lie-theory.md#binary-form) $F$ of degree $d\ge3$ and $m\ne0$. In a [splitting field](../../../galois-theory.md#splitting-field), write $F(X,Y)=a\prod_i(X-\rho_iY)$ and put $\theta_i=a\rho_i$, which are [algebraic integers](../../../algebraic-number-theory.md#algebraic-integer). The integral factors $L_i=aX-\theta_iY$ satisfy $\prod_iL_i=a^{d-1}m$. Each [ideal](../../../commutative-algebra.md#ideal) $(L_i)$ therefore divides one fixed [ideal](../../../commutative-algebra.md#ideal), giving finitely many possibilities. Choose a generator $\delta_i$ for each principal possibility, so $L_i=\delta_i u_i$ with [units](../../../algebra.md#unit-in-a-ring) $u_i$.

For three distinct roots,

$$
(\theta_2-\theta_3)L_1+(\theta_3-\theta_1)L_2+(\theta_1-\theta_2)L_3=0.
$$

Division by the third term gives a fixed-coefficient [unit](../../../algebra.md#unit-in-a-ring) equation in $u_1/u_3,u_2/u_3$. Its solutions are finite, hence there are finitely many values of $L_1/L_2$. This ratio determines the rational direction $X:Y$, since the roots are distinct. In a fixed direction, homogeneity and $F(X,Y)=m\ne0$ leave only finitely many [integer](../../../number-theory.md#integer) scales. This proves [Thue theorem](../../../number-theory.md#thue-theorem), and the argument also works for a form with at least three distinct projective roots even if reducible.

The hyperelliptic alternative uses a related factorization for the usual nondegenerate case with squarefree $f$ of degree at least three. For $y^2=f(x)$, [ideals](../../../commutative-algebra.md#ideal) of two different root factors can share primes only above the fixed root differences and the leading coefficient. At other primes their valuations are even. Finite exceptional-prime and ideal-class choices, together with [units](../../../algebra.md#unit-in-a-ring) modulo squares, reduce the factors to finitely many expressions $\delta_i z_i^2$. Relations between distinct root factors then give simultaneous norm or Pell-type equations. Writing their solutions in [fundamental units](../../../algebraic-number-theory.md#fundamental-unit-number-theory) and applying the same small-value/logarithmic-form estimates bounds the [unit](../../../algebra.md#unit-in-a-ring) exponents, hence $x,y$. The common-factor and square-class reductions are essential; a single quadratic norm equation alone can have infinitely many Pell solutions. This outlines the effective hyperelliptic treatment as well as the explicit Thue reduction.

## 6

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

The nondegenerate power-equation problem uses fixed positive $a,b$, fixed $c\ne0$, positive [integer](../../../number-theory.md#integer) bases, and exponents $n\ge3$. Lower exponents are separate: $n=1$ is linear, while $n=2$ can be a generalized [Pell equation](../../../number-theory.md#pell-equation) with infinitely many solutions. For example $x^2-2y^2=1$ has the infinite sequence generated by $(3+2\sqrt2)^j$. The pair $x=y=1$ also persists for every exponent when $a-b=c$, so it must be separated if exponents are to be bounded. For $n=1$, the [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm) gives a particular solution when $\gcd(a,b)\mid c$, and all solutions follow by adding multiples of $(b/\gcd(a,b),a/\gcd(a,b))$. For $n=2$, put $X=ax$ to obtain $X^2-ab y^2=ac$ with the congruence $a\mid X$. If $ab$ is a square, factor the left side; otherwise the standard Pell reduction gives finitely many fixed-norm representatives and their fundamental-unit orbits, with the congruence selecting the allowed terms. This is an effective description even when the set is infinite.

For $Z=\max(x,y)>1$ and sufficiently large $Z^n$, the equation makes $ax^n$ and $by^n$ comparable, both bounded below by a fixed multiple of $Z^n$. Their ratio gives

$$
\Lambda=\log(a/b)+n\log(x/y)=\log(1+c/(by^n))\ne0,\qquad\log|\Lambda|\le-n\log Z+O(1).
$$

If $x\ne y$, a two-logarithm estimate has one fixed algebraic argument $a/b$ and one variable rational argument $x/y$, of [arithmetic height](../../../algebraic-number-theory.md#height-function) at most $\log Z$. It gives $\log|\Lambda|\ge-C(a,b)\log Z\log(2n)$. A zero fixed logarithm is omitted, leaving the valid one-logarithm case. Therefore $n\le C\log(2n)+O(1)$, effectively bounding $n$. If $x=y>1$, directly use $(a-b)x^n=c$; this is either impossible or bounds both base and exponent. Cases where $Z^n$ stays small are finite and directly enumerable.

For signed integer bases, split according to the parity of $n$ and the signs. Cases reducing to a sum of positive powers are elementary because their sum is fixed; zero or absolute-value-one bases give separately detectable constant-power families.

For each bounded $n\ge3$, the form $aX^n-bY^n$ has $n$ distinct projective roots. The three-factor unit-equation argument of Question 5 gives an effective finite list of pairs, even if the binomial is reducible. Consequently **all nondegenerate solutions can be effectively found**, with the linear/Pell families and constant-base exception treated separately. This is the [exponent bound for a binomial power equation](../../../number-theory.md#exponent-bound-for-a-binomial-power-equation).

For the [polynomial](../../../polynomial.md) generalization the precise [Schinzel-Tijdeman exponent theorem](../../../number-theory.md#schinzel-tijdeman-exponent-theorem) is needed: if fixed $f\in\mathbb Q[X]$ has at least two distinct complex roots, solutions with [integers](../../../number-theory.md#integer) $x,y$, $|y|>1$, and $m\ge2$ have $m\le C(f)$ effectively. The hypotheses cannot be dropped. The one-root [polynomial](../../../polynomial.md) $f(X)=X^2$ gives $x=2^m$, $y=4$ for every $m$, and the two-root [polynomial](../../../polynomial.md) $f(X)=X(X-1)+1$ gives $x=0$, $y=1$ for every $m$.

To indicate the extension, factor $f$ over its [splitting field](../../../galois-theory.md#splitting-field) with root multiplicities $e_i$. Distinct factors have common [ideal](../../../commutative-algebra.md#ideal) [divisors](../../../number-theory.md#divisor) only over a fixed finite collection of primes. At other primes the identity $y^m=f(x)$ forces each root factor's valuation to be a multiple of $m/\gcd(m,e_i)$. [Ideal](../../../commutative-algebra.md#ideal) classes and [fundamental units](../../../algebraic-number-theory.md#fundamental-unit-number-theory) supply the remaining finitely specified factors. Generalized logarithmic-form estimates for these power equations control the [unit](../../../algebra.md#unit-in-a-ring) terms and exceptional primes and bound those reduced exponents; since $\gcd(m,e_i)\le e_i\le\deg f$, they bound $m$. This is why distinct roots and nontrivial perfect powers are indispensable to the asserted finiteness of exponents.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

The [abc conjecture](../../../number-theory.md#abc-conjecture) says that for every $\epsilon>0$ there is $C_\epsilon$ such that [coprime](../../../number-theory.md#coprime-integers) positive [integers](../../../number-theory.md#integer) $A+B=C$ satisfy $C\le C_\epsilon\operatorname{rad}(ABC)^{1+\epsilon}$, where the radical is the product of distinct prime [divisors](../../../number-theory.md#divisor).

The Catalan alternative yields finiteness of actual nontrivial solutions, with $x,y\ge2$ and $p,q\ge3$. Put $M=x^p$, so $y^q=M-1$ and $x,y$ are [coprime](../../../number-theory.md#coprime-integers). The triple $(y^q,1,x^p)$ has radical at most $xy<M^{2/3}$. Take $\epsilon=1/6$ to obtain

$$
M\le C_{1/6}M^{7/9},\qquad\boxed{M\le C_{1/6}^{9/2}}.
$$

Both bases are bounded, and $2^p\le M$, $2^q\le M-1$ also bound both exponents. Thus **only finitely many nontrivial Catalan solutions exist under abc**, the [Catalan power bound from abc](../../../number-theory.md#catalan-power-bound-from-abc).

For the Fermat alternative, the usual [arithmetic height](../../../algebraic-number-theory.md#height-function) statement concerns primitive solutions, or equivalently solutions modulo common scaling. A primitive positive triple is pairwise [coprime](../../../number-theory.md#coprime-integers), and $x,y<z$. Applying abc to $(x^n,y^n,z^n)$ gives

$$
z^n\le C_{1/6}(xyz)^{7/6}<C_{1/6}z^{7/2},\qquad\boxed{z\le C_{1/6}^2\quad(n\ge4)}.
$$

This is uniform even in $n$. If $h=\max(x,y)<z$, then $z^n=x^n+y^n\le2h^n$, so $n\le\log2/\log(z/h)$ is bounded after $z$ is bounded. There are therefore finitely many primitive triples and exponents, the [primitive Fermat bound from abc](../../../number-theory.md#primitive-fermat-bound-from-abc). Without the primitive convention, any one nonzero homogeneous solution would produce infinitely many common multiples. The Catalan proof above supplies the requested literal finiteness alternative without that normalization issue.

## 7

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

A [logarithmic form](../../../number-theory.md#linear-form-in-logarithms-of-algebraic-numbers) is $\Lambda=b_1\log\alpha_1+\cdots+b_s\log\alpha_s$ in fixed choices of logarithms of nonzero [algebraic numbers](../../../algebra.md#algebraic-number), with [integer](../../../number-theory.md#integer) coefficients. The indispensable condition is $\Lambda\ne0$. Put $B\ge\max(e,|b_1|,\ldots,|b_s|)$ and take $A_j\ge\max(Dh(\alpha_j),|\log\alpha_j|,1)$ for a [number field](../../../algebraic-number-theory.md#number-field) of degree $D$ containing the arguments. A typical effective estimate is

$$
\log|\Lambda|>-C(s,D)(1+\log B)\prod_j A_j,
$$

with an explicitly computable constant. For fixed arguments this is a power-type lower bound $|\Lambda|>B^{-C}$. It is fundamentally stronger for applications than a crude norm estimate exponential in $B$.

The basic estimates follow the auxiliary-function pattern already used here, in a multivariable form. Choose a [polynomial](../../../polynomial.md) or an interpolation determinant in powers of the algebraic arguments; impose many derivative or interpolation conditions by [Siegel lemma](../../../number-theory.md#siegel-s-lemma). Analytic extrapolation near the chosen logarithms makes the determinant tiny. Arithmetic denominator and norm estimates prevent a nonzero algebraic determinant from being so small, while a [multiplicity](../../../polynomial.md#multiplicity-mathematics) or zero estimate ensures the necessary determinant does not vanish identically. Balancing the degree, [multiplicity](../../../polynomial.md#multiplicity-mathematics) and [arithmetic height](../../../algebraic-number-theory.md#height-function) parameters produces dependence on the individual $A_j$ and only logarithmic dependence on $B$. The nonvanishing argument and the arithmetic [arithmetic height](../../../algebraic-number-theory.md#height-function) control are both necessary parts of this outline.

For practical equations the output is a finite, certified computation. Factor the equation in a [number field](../../../algebraic-number-theory.md#number-field), record the finitely many [ideal](../../../commutative-algebra.md#ideal) and torsion possibilities, and express its factors in [fundamental units](../../../algebraic-number-theory.md#fundamental-unit-number-theory). At a place where the original equation gives an exponentially small remainder, choose the principal logarithm and include a multiple of $2\pi i$ for the branch. Compare that upper bound with the effective lower bound to obtain an initial exponent bound. Question 5 shows this for a [unit](../../../algebra.md#unit-in-a-ring) equation, and Question 6 shows why a rational argument of variable [arithmetic height](../../../algebraic-number-theory.md#height-function) can still bound a common power exponent. Zero forms and degenerate families are separated before any estimate is applied.

A concrete two-logarithm example is $2^u-3^v=1$, with positive exponents. Here

$$
0<u\log2-v\log3=\log(1+3^{-v})<3^{-v}.
$$

The lower bound and $u=v\log3/\log2+O(1)$ give an effective upper bound for $u,v$. The exponents are [coprime](../../../number-theory.md#coprime-integers): a common [divisor](../../../number-theory.md#divisor) greater than one would factor a difference of two positive [integer](../../../number-theory.md#integer) powers equal to $1$, which is impossible. For large $v$ the same upper estimate makes $u/v$ a continued-fraction convergent of $\log3/\log2$, since its error is smaller than $1/(2v^2)$. One checks only the finitely many convergents up to the proven bound, with small cases checked directly. Higher-dimensional problems use the [LLL algorithm](../../../fourier-analysis.md#lenstra-lenstra-lovasz-lattice-basis-reduction-algorithm) to obtain analogous improvements from the first large bound.

Every numerical logarithm must be evaluated with a certified error interval, so that a proposed reduction really is an inequality and an exact [integer](../../../number-theory.md#integer) check can certify each surviving candidate. [Continued fractions](../../../number-theory.md#continued-fraction) or lattice reduction accelerate the search; the prior effective upper bound is what makes the search complete. This explains how [linear forms in logarithms of algebraic numbers](../../../number-theory.md#linear-form-in-logarithms-of-algebraic-numbers) turn qualitative finiteness into practical Diophantine algorithms, while also outlining the auxiliary machinery behind the estimates.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
