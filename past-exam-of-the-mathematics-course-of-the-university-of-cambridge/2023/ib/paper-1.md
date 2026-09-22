# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_1_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_1_2023.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3B](#3b)
  - [a](#3b/a)
    - [Solution](#3b/a/solution)
  - [b](#3b/b)
    - [Solution](#3b/b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5B](#5b)
  - [a](#5b/a)
    - [Solution](#5b/a/solution)
  - [b](#5b/b)
    - [Solution](#5b/b/solution)
- [6H](#6h)
  - [a](#6h/a)
    - [Solution](#6h/a/solution)
  - [b](#6h/b)
    - [Solution](#6h/b/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8F](#8f)
  - [a](#8f/a)
    - [Solution](#8f/a/solution)
  - [b](#8f/b)
    - [Solution](#8f/b/solution)
  - [c](#8f/c)
    - [Solution](#8f/c/solution)
  - [d](#8f/d)
    - [Solution](#8f/d/solution)
  - [e](#8f/e)
    - [Solution](#8f/e/solution)
- [9E](#9e)
  - [i](#9e/i)
    - [Solution](#9e/i/solution)
  - [ii](#9e/ii)
    - [Solution](#9e/ii/solution)
  - [iii](#9e/iii)
    - [Solution](#9e/iii/solution)
  - [iv](#9e/iv)
    - [Solution](#9e/iv/solution)
  - [Solution](#9e/solution)
- [10G](#10g)
  - [Solution](#10g/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12G](#12g)
  - [a](#12g/a)
    - [Solution](#12g/a/solution)
  - [b](#12g/b)
    - [Solution](#12g/b/solution)
  - [c](#12g/c)
    - [Solution](#12g/c/solution)
- [13A](#13a)
  - [a](#13a/a)
    - [Solution](#13a/a/solution)
  - [b](#13a/b)
    - [Solution](#13a/b/solution)
- [14D](#14d)
  - [a](#14d/a)
    - [Solution](#14d/a/solution)
  - [b](#14d/b)
    - [Solution](#14d/b/solution)
  - [c](#14d/c)
    - [Solution](#14d/c/solution)
  - [d](#14d/d)
    - [Solution](#14d/d/solution)
- [15D](#15d)
  - [Solution](#15d/solution)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [Solution](#15d/b/solution)
  - [c](#15d/c)
    - [Solution](#15d/c/solution)
  - [d](#15d/d)
    - [Solution](#15d/d/solution)
  - [e](#15d/e)
    - [Solution](#15d/e/solution)
- [16C](#16c)
  - [a](#16c/a)
    - [i](#16c/a/i)
      - [Solution](#16c/a/i/solution)
    - [ii](#16c/a/ii)
      - [Solution](#16c/a/ii/solution)
  - [b](#16c/b)
    - [i](#16c/b/i)
      - [Solution](#16c/b/i/solution)
    - [ii](#16c/b/ii)
      - [Solution](#16c/b/ii/solution)
    - [iii](#16c/b/iii)
      - [Solution](#16c/b/iii/solution)
    - [iv](#16c/b/iv)
      - [Solution](#16c/b/iv/solution)
- [17B](#17b)
  - [a](#17b/a)
    - [Solution](#17b/a/solution)
  - [b](#17b/b)
    - [Solution](#17b/b/solution)
  - [c](#17b/c)
    - [Solution](#17b/c/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)
  - [e](#18h/e)
    - [Solution](#18h/e/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)
  - [c](#19h/c)
    - [Solution](#19h/c/solution)

## 1F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

Choose [bases](../../../vector-space.md#basis) of $V$ and $W$, of dimensions $v$ and $w$. A [linear map](../../../vector-space.md#linear-map) is uniquely determined by the arbitrary images of the $v$ [basis](../../../vector-space.md#basis) [vectors](../../../vector-space.md#vector), each with $w$ coordinates, so

$$
\dim L(V,W)=vw.
$$

Put $a=\dim A$ and $b=\dim B$, and extend [bases](../../../vector-space.md#basis) of $A,B$ to [bases](../../../vector-space.md#basis) of $V,W$. The condition $\phi(A)\subseteq B$ forces the $(w-b)a$ [matrix](../../../vector-space.md#matrix) entries from $A$ to a complement of $B$ to vanish and imposes no other restriction. Hence

$$
\dim X=vw-a(w-b).
$$

For the last part let $r=\dim(S\cap T)=s+t-v$. Choose

$$
V=(S\cap T)\oplus S_0\oplus T_0.
$$

A map in $Y$ sends $S\cap T$ into itself, $S_0$ into $S$, and $T_0$ into $T$, with these choices independent. Therefore

$$
\boxed{\dim Y=r^2+s(s-r)+t(t-r),
\qquad r=s+t-v.}
$$

## 2F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

A [topological surface](../../../topology.md#topological-surface) is a Hausdorff, second-countable space in which every point has a neighbourhood homeomorphic to an open subset of $\mathbb R^2$.

The antipodal action on $S^2$ is free. The [surface quotient by a free finite action](../../../topology.md#surface-quotient-by-a-free-finite-action) applies: Around each point choose a small [open disc](../../../topology.md#open-disc) disjoint from its antipodal image; the quotient map restricts to a homeomorphism from that disc onto an open neighbourhood in the quotient. Compactness gives Hausdorffness and second countability descends from the sphere. Thus the quotient is the [real projective plane](../../../differential-geometry.md#real-projective-plane), in particular a topological surface.

For the second quotient write a point away from the poles as

$$
(\sqrt{1-z^2}\cos\phi,\sqrt{1-z^2}\sin\phi,z).
$$

The map

$$
q(\phi,z)=(2\phi,z)
$$

in these cylindrical coordinates extends continuously over the poles and identifies exactly $\phi$ with $\phi+\pi$. It therefore induces a continuous bijection $S^2/\!\approx\,\to S^2$. The domain is compact and the sphere Hausdorff, so this bijection is a homeomorphism.

## 3B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3b/a">a</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/a/solution">Solution</h4>

↑ **Parent:** [A](#3b/a)

The [Laurent series](../../../analysis.md#laurent-series) is

$$
e^{1/z}=\sum_{k=0}^{\infty}\frac{1}{k!z^k},
\qquad 0<|z|<\infty.
$$

**Thus zero is an essential singularity.**

<h3 id="3b/b">b</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/b/solution">Solution</h4>

↑ **Parent:** [B](#3b/b)

On $|z|\geq\rho$, put $w=1/z$, so $|w|\leq1/\rho$. The Taylor [polynomials](../../../polynomial.md)

$$
f_n(z)=\sum_{k=0}^n\frac{w^k}{k!}
$$

converge uniformly there to $e^w$. Moreover

$$
|e^w|=e^{\Re w}\geq e^{-1/\rho}.
$$

For all sufficiently large $n$, the uniform error is below half this lower bound, so $|f_n(z)|>0$ whenever $|z|\geq\rho$. Every zero therefore lies in $|z|<\rho$.

## 4C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For a regular constraint $g=0$, an interior constrained extremum satisfies

$$
\nabla f=\lambda\nabla g,
$$

together with the constraint; boundary cases must also be checked.

Here maximize $f=xyz$ subject to $x^2+y^2+z^2=L^2$. The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations give

$$
yz=2\lambda x,\qquad xz=2\lambda y,\qquad xy=2\lambda z.
$$

At a positive maximizer these imply $x=y=z=L/\sqrt3$. Boundary points have zero volume, so the maximum is

$$
\boxed{\frac{L^3}{3\sqrt3}}.
$$

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/a">a</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/a/solution">Solution</h4>

↑ **Parent:** [A](#5b/a)

For any $h$,

$$
\|A(c^*+h)-y\|_2^2
=\|Ac^*-y\|_2^2+2h^TA^T(Ac^*-y)+\|Ah\|_2^2.
$$

If the [normal equation](../../../statistical-modelling.md#normal-equation) $A^TAc^*=A^Ty$ holds, the last two terms reduce to $\|Ah\|^2\geq0$, so $c^*$ minimizes. Conversely, at a minimizer the directional [derivative](../../../calculus.md#derivative) in every $h$ vanishes, forcing $A^T(Ac^*-y)=0$.

<h3 id="5b/b">b</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/b/solution">Solution</h4>

↑ **Parent:** [B](#5b/b)

If $A$ has full column rank, then for every nonzero $h$,

$$
h^TA^TAh=\|Ah\|^2>0.
$$

Thus $A^TA$ is positive definite and invertible, and the normal equation has the unique solution

$$
\boxed{c^*=(A^TA)^{-1}A^Ty.}
$$

## 6H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6h/a">a</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/a/solution">Solution</h4>

↑ **Parent:** [A](#6h/a)

For a null parameter space $\Theta_0\subseteq\Theta$, the generalized likelihood ratio is

$$
\Lambda=\frac{\sup_{\theta\in\Theta_0}L(\theta)}
{\sup_{\theta\in\Theta}L(\theta)}.
$$

The [Wilks theorem](../../../statistical-inference.md#wilks-theorem) states, under standard regularity conditions and under the null, that

$$
-2\log\Lambda\Rightarrow\chi^2_{\dim\Theta-\dim\Theta_0}.
$$

<h3 id="6h/b">b</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/b/solution">Solution</h4>

↑ **Parent:** [B](#6h/b)

The null hypothesis is that mortality is independent of carbolic-acid use, equivalently that the two mortality probabilities are equal. The two-sided alternative is that they differ.

Use the [Chi-squared test of independence](../../../statistical-inference.md#chi-squared-test-of-independence), equivalently the likelihood-ratio statistic, with Pearson's statistic

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}},
$$

where $E_{ij}$ are the fitted counts under independence using the observed row and column totals. Under the null, $X^2$ is asymptotically $\chi^2_1$. A size-$\alpha$ test rejects when

$$
\boxed{X^2>\chi^2_{1,1-\alpha}.}
$$

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

The [minimum-cost flow](../../../graph-theory.md#minimum-cost-flow-problem) problem chooses, for each directed edge $(i,j)\in E$, a flow $x_{ij}$ and solves

$$
\min_x\sum_{(i,j)\in E}C_{ij}x_{ij}
$$

subject to

$$
\sum_{j:(j,i)\in E}x_{ji}-\sum_{j:(i,j)\in E}x_{ij}=b_i,
\qquad
M_{ij}\leq x_{ij}\leq\overline M_{ij}.
$$

Feasibility requires $\sum_i b_i=0$.

Set $y_{ij}=x_{ij}-M_{ij}$. Then

$$
0\leq y_{ij}\leq\overline M_{ij}-M_{ij},
$$

and its balance [vector](../../../vector-space.md#vector) is

$$
b_i'=b_i+\sum_jM_{ij}-\sum_jM_{ji}.
$$

The objective becomes $\sum C_{ij}y_{ij}$ plus the constant $\sum C_{ij}M_{ij}$. Translation by $M$ is a bijection between feasible flows and preserves their ordering by cost, so the transformed zero-lower-bound problem is equivalent.

## 8F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8f/a">a</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/a/solution">Solution</h4>

↑ **Parent:** [A](#8f/a)

**True.** By [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form), the characteristic [polynomial](../../../polynomial.md) records the total size of the blocks for each [eigenvalue](../../../linear-operator-theory.md#eigenvalue), while the minimal [polynomial](../../../polynomial.md) records the largest block for each [eigenvalue](../../../linear-operator-theory.md#eigenvalue). In dimension three this determines every block partition: for algebraic multiplicity three the possibilities $3$, $2+1$, and $1+1+1$ have largest block sizes three, two, and one; multiplicities one and two are equally immediate. Thus the two [matrices](../../../vector-space.md#matrix) have the same Jordan form and are conjugate. This is the [characteristic and minimal polynomials determine similarity in dimension three](../../../linear-operator-theory.md#characteristic-and-minimal-polynomials-determine-similarity-in-dimension-three) phenomenon.

<h3 id="8f/b">b</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/b/solution">Solution</h4>

↑ **Parent:** [B](#8f/b)

**False.** At [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $2$, algebraic multiplicity two and minimal-polynomial exponent two force one block $J_2(2)$. At [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$, the blocks have total size five and largest size two, so there are only two possible partitions,

$$
2+2+1\qquad\hbox{or}\qquad2+1+1+1.
$$

Hence there are exactly two conjugacy classes satisfying the given [polynomial](../../../polynomial.md) data, represented by

$$
J_2(2)\oplus J_2(1)\oplus J_2(1)\oplus J_1(1)
$$

and

$$
J_2(2)\oplus J_2(1)\oplus J_1(1)\oplus J_1(1)\oplus J_1(1).
$$

There cannot be three mutually non-conjugate examples.

<h3 id="8f/c">c</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/c/solution">Solution</h4>

↑ **Parent:** [C](#8f/c)

**True.** Since $\alpha$ is invertible, every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ is nonzero. If $\alpha$ had a nontrivial Jordan block $\lambda I+N$, then for the stated positive integer $N_0$,

$$
(\lambda I+N)^{N_0}
=\lambda^{N_0}I+N_0\lambda^{N_0-1}N+\cdots
$$

would still have a nonzero nilpotent part and could not be diagonalizable. Therefore all Jordan blocks of $\alpha$ have size one. This also proves [diagonalizability inherited from an invertible power](../../../linear-operator-theory.md#diagonalizability-inherited-from-an-invertible-power).

<h3 id="8f/d">d</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/d/solution">Solution</h4>

↑ **Parent:** [D](#8f/d)

**False.** The real [matrix](../../../vector-space.md#matrix)

$$
A=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

has the two distinct complex [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $i$ and $-i$, so it is diagonalizable over $\mathbb C$. It has no real [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and hence no real eigenbasis, so it is not diagonalizable over $\mathbb R$.

<h3 id="8f/e">e</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/e/solution">Solution</h4>

↑ **Parent:** [E](#8f/e)

**True.** Suppose $A,B$ are real and $AP=PB$ for an invertible complex [matrix](../../../vector-space.md#matrix) $P=X+iY$, with $X,Y$ real. Taking real and imaginary parts gives

$$
AX=XB,\qquad AY=YB.
$$

The [polynomial](../../../polynomial.md) $q(t)=\det(X+tY)$ is not identically zero, since $q(i)=\det P\ne0$. Choose a real $t$ outside its finite zero set. Then $Q=X+tY$ is real and invertible, and $AQ=QB$. Thus $A$ and $B$ are conjugate over $\mathbb R$, as stated by [complex similarity of real matrices implies real similarity](../../../linear-operator-theory.md#complex-similarity-of-real-matrices-implies-real-similarity).

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/i">i</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/i/solution">Solution</h4>

↑ **Parent:** [I](#9e/i)

Assume (i). For $a,b\in R$, write the [ideal](../../../commutative-algebra.md#ideal) $(a,b)=(d)$. Then $d=ra+sb$ for some $r,s\in R$. Since $a,b\in(d)$, the element $d$ divides both; and every common divisor of $a,b$ divides the displayed linear combination $d$. Thus $d$ is a greatest common divisor and (ii) holds.

<h3 id="9e/ii">ii</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9e/ii)

Assume (ii), and let an $R$-submodule $M\subseteq F$ be generated by $x_1,\ldots,x_m$. Choose a common nonzero denominator $d$ and write $x_j=a_j/d$ with $a_j\in R$. Repeated application of (ii) shows that

$$
(a_1,\ldots,a_m)=(g)
$$

for one element $g$: the gcd at each step is a linear combination of the elements processed so far. Therefore

$$
M=R\frac gd,
$$

so (iii) holds. This is the finite-ideal property defining a [Bézout domain](../../../commutative-algebra.md#bezout-domain).

<h3 id="9e/iii">iii</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9e/iii)

Assume (iii). Because $R$ is a [Noetherian ring](../../../algebra.md#noetherian-ring), every [ideal](../../../commutative-algebra.md#ideal) $I\subseteq R$ is finitely generated. Regard $I$ as an $R$-submodule of $F$. By (iii), $I=Rx$ for some $x\in F$; since $x\in I\subseteq R$ unless $I=0$, this is a principal [ideal](../../../commutative-algebra.md#ideal) of $R$. Thus every [ideal](../../../commutative-algebra.md#ideal) is principal and (i) holds.

Together with the previous two implications, this proves (i), (ii), and (iii) equivalent.

<h3 id="9e/iv">iv</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#9e/iv)

If (i) holds, the [submodule theorem for free modules over a principal ideal domain](../../../commutative-algebra.md#submodule-theorem-for-free-modules-over-a-principal-ideal-domain) says that any submodule $N\subseteq R^n$ is free. Its rank is at most $n$, since tensoring the inclusion with $F$ embeds $N\otimes_R F$ into $F^n$. Hence $N$ has at most $n$ generators, proving (iv).

Conversely, apply (iv) with $n=1$. Every [ideal](../../../commutative-algebra.md#ideal) is an $R$-submodule of $R$ and therefore has one generator, which is (i). Thus all four conditions are equivalent.

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

Suppose the additive [group](../../../group.md) of the [integral](../../../calculus.md#integral) domain $R$ is isomorphic to $\mathbb Z^n$. Every [ideal](../../../commutative-algebra.md#ideal) $I$ is then an additive [subgroup](../../../group.md#subgroup) of a finitely generated free abelian [group](../../../group.md), so it has finitely many additive generators $x_1,\ldots,x_m$. These also generate $I$ as an $R$-ideal: integer coefficients are coefficients from the canonical copy of $\mathbb Z$ in $R$. Thus every [ideal](../../../commutative-algebra.md#ideal) is finitely generated, proving that $R$ is Noetherian by [noetherianity from finite additive rank](../../../algebra.md#noetherianity-from-finite-additive-rank).

For an example that fails (i)--(iv), take

$$
R=\mathbb Z[\sqrt{-5}].
$$

It is an [integral](../../../calculus.md#integral) domain and has additive [group](../../../group.md) $\mathbb Z^2$. The [ideal](../../../commutative-algebra.md#ideal)

$$
I=(2,1+\sqrt{-5})
$$

has index two: modulo $I$, one has $2=0$ and $\sqrt{-5}=-1=1$, and the resulting quotient is $\mathbb F_2$. If $I=(a+b\sqrt{-5})$, multiplication by its generator would have [determinant](../../../linear-algebra.md#determinant) and absolute index

$$
a^2+5b^2=2,
$$

which has no integer solution. Hence $I$ is not principal, as detailed in [nonprincipal ideal in the integers adjoined a square root of minus five](../../../algebra.md#nonprincipal-ideal-in-the-integers-adjoined-a-square-root-of-minus-five). Condition (i), and therefore all four equivalent conditions, fails.

## 10G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10g/solution">Solution</h3>

↑ **Parent:** [10G](#10g)

A [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) $(x_n)$ in a metric space $(M,d)$ satisfies: for every $\varepsilon>0$ there is $N$ such that $d(x_m,x_n)<\varepsilon$ whenever $m,n\geq N$. A [complete metric space](../../../topological-analysis.md#complete-metric-space) is one in which every Cauchy [sequence](../../../real-analysis.md#sequence) converges to a point of the space.

Every Cauchy [sequence](../../../real-analysis.md#sequence) is bounded. Choose $N$ such that $d(x_n,x_N)<1$ for $n\geq N$, and put

$$
R=1+\max_{1\leq j<N}d(x_j,x_N).
$$

Then every term lies in the ball $B(x_N,R)$.

Now suppose $M$ is complete and $(F_n)$ is a decreasing [sequence](../../../real-analysis.md#sequence) of nonempty closed sets with $\operatorname{diam}F_n\to0$. Choose $x_n\in F_n$. Given $\varepsilon>0$, choose $N$ with $\operatorname{diam}F_N<\varepsilon$. For $m,n\geq N$, both points lie in $F_N$, so $d(x_m,x_n)<\varepsilon$. Completeness gives $x_n\to x\in M$. For each fixed $N$, the tail lies in the closed set $F_N$, hence $x\in F_N$. Therefore

$$
x\in\bigcap_{n=1}^{\infty}F_n.
$$

Conversely, assume the nested-set property and let $(x_n)$ be Cauchy. Define

$$
F_n=\overline{\{x_m:m\geq n\}}.
$$

These sets are nonempty, closed, and decreasing. The Cauchy property implies $\operatorname{diam}F_n\to0$; taking a closure does not change the diameter. Choose $x\in\bigcap_nF_n$. Since $x_n,x\in F_n$,

$$
d(x_n,x)\leq\operatorname{diam}F_n\longrightarrow0.
$$

Thus every Cauchy [sequence](../../../real-analysis.md#sequence) converges and $M$ is complete. This proves the [Cantor intersection theorem](../../../topological-analysis.md#cantor-s-intersection-theorem) characterization.

The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) states that a contraction of a nonempty complete metric space has a unique fixed point.

For each $\lambda\in\Lambda$, the map $T_\lambda(x)=T(\lambda,x)$ is a contraction with the common constant $k$, so it has a unique fixed point $x^*(\lambda)$. This defines the required unique [function](../../../function.md). Fix $\lambda_0$. The fixed-point identities and the triangle inequality give

$$
\begin{aligned}
d(x^*(\lambda),x^*(\lambda_0))
&\leq d(T(\lambda,x^*(\lambda)),T(\lambda,x^*(\lambda_0)))\\
&\quad+d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0)))\\
&\leq k\,d(x^*(\lambda),x^*(\lambda_0))
+d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0))).
\end{aligned}
$$

Consequently

$$
d(x^*(\lambda),x^*(\lambda_0))
\leq\frac{d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0)))}{1-k}.
$$

The numerator tends to zero as $\lambda\to\lambda_0$ by the assumed continuity for the fixed point $x^*(\lambda_0)$. Hence $x^*$ is continuous, an instance of [continuous dependence of the fixed point of a uniform contraction](../../../analysis.md#continuous-dependence-of-the-fixed-point-of-a-uniform-contraction).

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

A subset $S\subset\mathbb R^3$ is a smooth surface if every point has a neighbourhood in $S$ parametrized by a map $X:U\to S$, where $U\subset\mathbb R^2$ is open, $X$ is a homeomorphism onto that neighbourhood, $X$ is smooth, and $DX$ has rank two everywhere. These are the [embedded surface parametrization](../../../differential-geometry.md#embedded-surface-parametrization) conditions.

For the given set use local angular intervals in the parametrization

$$
X(\theta,t)=(\phi(t)\cos\theta,\phi(t)\sin\theta,t).
$$

It is locally one-to-one and has [tangent vectors](../../../differential-geometry.md#tangent-vector)

$$
X_\theta=(-\phi\sin\theta,\phi\cos\theta,0),
\qquad
X_t=(\phi'\cos\theta,\phi'\sin\theta,1).
$$

Their cross product has magnitude

$$
|X_\theta\times X_t|=\phi(t)\sqrt{1+\phi'(t)^2}>0,
$$

so the [derivative](../../../calculus.md#derivative) has rank two. The angular charts cover $\Sigma$, proving that it is a smooth surface.

The area between heights $a_0$ and $b_0$ is therefore

$$
2\pi\int_{a_0}^{b_0}\phi(t)\sqrt{1+\phi'(t)^2}\,dt.
$$

By hypothesis this equals $2\pi r(b_0-a_0)$ for every subinterval. Since the integrand is continuous,

$$
\phi(t)\sqrt{1+\phi'(t)^2}=r,
$$

and squaring gives

$$
r^2=\phi(t)^2+\phi(t)^2\phi'(t)^2.
$$

If $0<\phi(t)<r$, then $\phi'$ never vanishes, so its sign $\sigma\in\{1,-1\}$ is constant. The last equation gives

$$
\phi'=\sigma\frac{\sqrt{r^2-\phi^2}}{\phi},
$$

and hence

$$
\frac d{dt}\sqrt{r^2-\phi(t)^2}=-\sigma.
$$

Thus $\sqrt{r^2-\phi(t)^2}=-\sigma(t-t_0)$ for a constant $t_0$, and

$$
(t-t_0)^2+\phi(t)^2=r^2.
$$

The graph lies on a circle of radius $r$, exactly as described by [constant strip-area density of a surface of revolution](../../../differential-geometry.md#constant-strip-area-density-of-a-surface-of-revolution).

## 12G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12g/a">a</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/a/solution">Solution</h4>

↑ **Parent:** [A](#12g/a)

Termwise [differentiation](../../../calculus.md#differentiation) inside the disc gives

$$
f'(z)=\sum_{n=1}^{\infty}(1-z)^{n-1}=\frac1z.
$$

Consequently

$$
\frac d{dz}\bigl(ze^{-f(z)})
=e^{-f(z)}(1-zf'(z))=0.
$$

Since $f(1)=0$, the constant is one, so $e^{f(z)}=z$. Thus $f$ is an analytic branch of the logarithm on $D(1,1)$ with the required value.

Given $a\in D$, write $a=|a|e^{i\theta_a}$ with $0<\theta_a<2\pi$. On $|z/a-1|<1$, define

$$
\ell_a(z)=f(z/a)+\log|a|+i\theta_a.
$$

Then $e^{\ell_a(z)}=z$ and $\operatorname{Im}\ell_a(a)=\theta_a$. After shrinking the neighbourhood of $a$, continuity keeps its imaginary part in $(0,2\pi)$.

<h3 id="12g/b">b</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/b/solution">Solution</h4>

↑ **Parent:** [B](#12g/b)

Near each $a\in D$, the local branch from part (a), chosen to have value $\log|a|+i\theta(a)$ at $a$, agrees with

$$
L(z)=\log|z|+i\theta(z).
$$

Indeed, two logarithms of the same nonzero number differ by $2\pi i$ times an integer, and the integer is locally constant; it is zero at $a$. Hence $L$ is locally analytic and therefore analytic on $D$. This is the [analytic logarithm on the positive-axis slit plane](../../../analysis.md#analytic-logarithm-on-the-positive-axis-slit-plane).

For $-1<\alpha<1$, an analytic branch is

$$
\boxed{z^\alpha=\exp(\alpha L(z)).}
$$

<h3 id="12g/c">c</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/c/solution">Solution</h4>

↑ **Parent:** [C](#12g/c)

The [residue theorem](../../../analysis.md#residue-theorem) states that if a meromorphic [function](../../../function.md) has finitely many poles inside a positively oriented simple closed contour and none on it, then its contour [integral](../../../calculus.md#integral) is $2\pi i$ times the sum of the enclosed residues.

Apply it to

$$
F(z)=\frac{e^{\alpha L(z)}}{(1+z)^2}
$$

on a keyhole contour around the positive real axis. The outer and inner circles vanish as their radii tend to infinity and zero because $\alpha<1$ and $\alpha>-1$, respectively. On the upper bank the numerator tends to $x^\alpha$, while on the lower bank it tends to $e^{2\pi i\alpha}x^\alpha$ and the direction is reversed. Therefore the limiting contour [integral](../../../calculus.md#integral) is

$$
(1-e^{2\pi i\alpha})I.
$$

The only enclosed pole is the double pole at $z=-1$. Since $L(-1)=i\pi$,

$$
\operatorname{Res}_{z=-1}F
=\left.\frac d{dz}e^{\alpha L(z)}\right|_{z=-1}
=-\alpha e^{i\pi\alpha}.
$$

The residue theorem now gives

$$
(1-e^{2\pi i\alpha})I=-2\pi i\alpha e^{i\pi\alpha}.
$$

For $\alpha\ne0$, division and

$$
1-e^{2\pi i\alpha}=-2ie^{i\pi\alpha}\sin(\pi\alpha)
$$

yield

$$
\boxed{I=\frac{\pi\alpha}{\sin(\pi\alpha)}}.
$$

At $\alpha=0$, the [integral](../../../calculus.md#integral) is one, agreeing with the continuous [limit](../../../calculus.md#limit-of-a-function). This is the [positive-axis keyhole beta integral](../../../analysis.md#positive-axis-keyhole-beta-integral).

## 13A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13a/a">a</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/a/solution">Solution</h4>

↑ **Parent:** [A](#13a/a)

The Lagrange identity for this [Sturm-Liouville theory](../../../analysis.md#sturm-liouville-theory) operator is

$$
y_0L(y;\lambda_0)-yL(y_0;\lambda_0)
=\frac d{dx}\left[p(y_0y'-yy_0')\right].
$$

Integrating from zero to one, the boundary term vanishes because both $y$ and $y_0$ vanish at both endpoints. Since $L(y_0;\lambda_0)=0$ and $L(y;\lambda_0)=f$, it follows that

$$
\int_0^1y_0f\,dx=0.
$$

This is the [solvability condition at a Sturm-Liouville eigenvalue](../../../analysis.md#solvability-condition-at-a-sturm-liouville-eigenvalue).

<h3 id="13a/b">b</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/b/solution">Solution</h4>

↑ **Parent:** [B](#13a/b)

Because the parameter enters through $\lambda wy$,

$$
L(y;\lambda_0)
=L(y;\lambda)-(\lambda-\lambda_0)wy
=y^{m+1}-\varepsilon^m\mu wy.
$$

Use this as $f$ in part (a). The necessary orthogonality condition is

$$
0=\int_0^1y_0\left(y^{m+1}-\varepsilon^m\mu wy\right)dx.
$$

With $y=\varepsilon y_0+\varepsilon^2y_1$ and $\mu=O(1)$,

$$
y^{m+1}=\varepsilon^{m+1}y_0^{m+1}+O(\varepsilon^{m+2}),
\qquad
wy=\varepsilon wy_0+O(\varepsilon^2).
$$

Consequently

$$
0=\varepsilon^{m+1}
\left[
\int_0^1y_0^{m+2}\,dx
-\mu\int_0^1wy_0^2\,dx
\right]
+O(\varepsilon^{m+2}).
$$

The normalization makes the second [integral](../../../calculus.md#integral) one. Divide by $\varepsilon^{m+1}$ to obtain

$$
\boxed{\mu=\int_0^1y_0^{m+2}\,dx+O(\varepsilon)}.
$$

This is the [leading nonlinear eigenvalue shift in a Sturm-Liouville problem](../../../analysis.md#leading-nonlinear-eigenvalue-shift-in-a-sturm-liouville-problem).

## 14D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14d/a">a</h3>

↑ **Parent:** [14D](#14d)

<h4 id="14d/a/solution">Solution</h4>

↑ **Parent:** [A](#14d/a)

For a normalized state, write

$$
A'=\widehat A-\langle\widehat A\rangle_\psi,
\qquad
B'=\widehat B-\langle\widehat B\rangle_\psi.
$$

Then $\Delta_\psi A=\|A'\psi\|$ and $\Delta_\psi B=\|B'\psi\|$. The Schwarz inequality gives

$$
(\Delta_\psi A)(\Delta_\psi B)
\geq |(A'\psi,B'\psi)|
\geq |\operatorname{Im}(A'\psi,B'\psi)|.
$$

Since $A'$ and $B'$ are Hermitian and their commutator equals $[\widehat A,\widehat B]$,

$$
2i\operatorname{Im}(A'\psi,B'\psi)
=(\psi,[\widehat A,\widehat B]\psi).
$$

Therefore

$$
(\Delta_\psi A)(\Delta_\psi B)
\geq\frac12\left|(\psi,[\widehat A,\widehat B]\psi)\right|,
$$

which is the [Robertson uncertainty principle](../../../quantum-theory.md#robertson-uncertainty-principle).

<h3 id="14d/b">b</h3>

↑ **Parent:** [14D](#14d)

<h4 id="14d/b/solution">Solution</h4>

↑ **Parent:** [B](#14d/b)

Because $\widehat X-i\lambda\widehat Y$ is the adjoint of $\widehat X+i\lambda\widehat Y$,

$$
f(\lambda)=\|(\widehat X+i\lambda\widehat Y)\psi\|^2\geq0.
$$

Expanding gives the real quadratic

$$
f(\lambda)
=\langle\widehat X^2\rangle
+i\lambda\langle[\widehat X,\widehat Y]\rangle
+\lambda^2\langle\widehat Y^2\rangle.
$$

Its discriminant must be nonpositive. Since the expectation of a commutator of Hermitian operators is purely imaginary,

$$
4\langle\widehat X^2\rangle\langle\widehat Y^2\rangle
\geq\left|\langle[\widehat X,\widehat Y]\rangle\right|^2.
$$

Taking $\widehat X=\widehat A-\langle\widehat A\rangle$ and $\widehat Y=\widehat B-\langle\widehat B\rangle$ and then taking square roots gives the stated uncertainty relation. This is the [quadratic-norm proof of the Heisenberg uncertainty relation](../../../quantum-theory.md#quadratic-norm-proof-of-the-heisenberg-uncertainty-relation).

<h3 id="14d/c">c</h3>

↑ **Parent:** [14D](#14d)

<h4 id="14d/c/solution">Solution</h4>

↑ **Parent:** [C](#14d/c)

For a [differentiable](../../../analysis.md#differentiable-function) wave [function](../../../function.md),

$$
[\widehat x,\widehat p]\psi
=-i\hbar x\psi'+i\hbar(x\psi)'
=i\hbar\psi.
$$

Thus $[\widehat x,\widehat p]=i\hbar I$. Substitution into part (a) yields

$$
\boxed{\Delta_\psi x\,\Delta_\psi p\geq\frac\hbar2}.
$$

<h3 id="14d/d">d</h3>

↑ **Parent:** [14D](#14d)

<h4 id="14d/d/solution">Solution</h4>

↑ **Parent:** [D](#14d/d)

For $\psi(x)=Ce^{-\alpha x^2}$,

$$
\psi''=(4\alpha^2x^2-2\alpha)\psi.
$$

The stationary [Schrödinger equation](../../../physics.md#schrodinger-equation) becomes

$$
\left[
\frac{\hbar^2\alpha}{m}
+\left(k-\frac{2\hbar^2\alpha^2}{m}\right)x^2
\right]\psi=E\psi.
$$

Hence, choosing the positive root and a positive normalization constant,

$$
\alpha=\frac1\hbar\sqrt{\frac{mk}{2}},
\qquad
E=\hbar\sqrt{\frac{k}{2m}},
\qquad
C=\left(\frac{2\alpha}{\pi}\right)^{1/4}.
$$

The state is even, so $\langle x\rangle=\langle p\rangle=0$. The Gaussian [integrals](../../../calculus.md#integral) give

$$
(\Delta x)^2=\frac1{4\alpha},
\qquad
(\Delta p)^2=\hbar^2\alpha,
$$

and therefore $\Delta x\Delta p=\hbar/2$. These values are collected in [gaussian eigenstate for a quadratic potential](../../../quantum-theory.md#gaussian-eigenstate-for-a-quadratic-potential).

Finally, equality in the derivation of the uncertainty relation requires the centred [vectors](../../../vector-space.md#vector) to be linearly dependent with a purely imaginary proportionality constant. Thus for some $s>0$,

$$
(\widehat p-p_0)\psi=is(\widehat x-x_0)\psi.
$$

In position space this says

$$
\psi'=\left(\frac{ip_0}{\hbar}-\frac{s(x-x_0)}{\hbar}\right)\psi,
$$

whose normalizable solutions are

$$
\psi(x)=C_0\exp\left(\frac{ip_0x}{\hbar}-\frac{s(x-x_0)^2}{2\hbar}\right).
$$

**Thus every saturating state is Gaussian up to translation, a plane-wave factor, and an overall phase, as in the [equality case of the Heisenberg uncertainty relation](../../../quantum-theory.md#equality-case-of-the-heisenberg-uncertainty-relation).**

## 15D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15d/solution">Solution</h3>

↑ **Parent:** [15D](#15d)

In SI units the [Maxwell equations](../../../electromagnetism.md#maxwell-equations) in free space are

$$
\nabla\cdot E=\frac{\rho}{\epsilon_0},
\qquad
\nabla\cdot B=0,
$$



$$
\nabla\times E=-\frac{\partial B}{\partial t},
\qquad
\nabla\times B=\mu_0J+\mu_0\epsilon_0\frac{\partial E}{\partial t}.
$$

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

Take the divergence of the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law). Since the divergence of a curl is zero, [Gauss's law](../../../electromagnetism.md#gauss-s-law) gives

$$
0=\mu_0\nabla\cdot J
+\mu_0\epsilon_0\frac{\partial}{\partial t}(\nabla\cdot E)
=\mu_0\left(\nabla\cdot J+\frac{\partial\rho}{\partial t}\right).
$$

Thus

$$
\frac{\partial\rho}{\partial t}+\nabla\cdot J=0,
$$

which is [charge conservation from Maxwell equations](../../../electromagnetism.md#charge-conservation-from-maxwell-equations). Integrating over a fixed volume and using the divergence theorem yields

$$
\frac{dQ}{dt}=-\int_{\partial V}J\cdot n\,dS.
$$

Charge in $V$ is conserved provided no current crosses $\partial V$. For total charge in all space, the corresponding assumption is sufficient decay of $J$ so that the flux at infinity vanishes.

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/solution">Solution</h4>

↑ **Parent:** [B](#15d/b)

In empty space the fields are divergence-free. Taking the curl of [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) and using

$$
\nabla\times(\nabla\times E)=\nabla(\nabla\cdot E)-\nabla^2E
$$

gives

$$
\nabla^2E-\mu_0\epsilon_0\frac{\partial^2E}{\partial t^2}=0.
$$

The same calculation, starting from the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law), gives the corresponding equation for $B$. Thus every component satisfies the [electromagnetic wave equation](../../../electromagnetism.md#electromagnetic-wave-equation) with speed

$$
c=\frac1{\sqrt{\mu_0\epsilon_0}}
\simeq3.0\times10^8\ \mathrm{m\,s^{-1}}.
$$

Its agreement with the measured speed of light identifies light as an [electromagnetic wave](../../../electromagnetism.md#electromagnetic-wave).

<h3 id="15d/c">c</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/c/solution">Solution</h4>

↑ **Parent:** [C](#15d/c)

Dot the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) with $E$, dot [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) with $B/\mu_0$, and use the stated [vector](../../../vector-space.md#vector) identity. The result is the local balance law

$$
\frac{\partial}{\partial t}
\left[
\frac12\left(\epsilon_0E^2+\frac{B^2}{\mu_0}\right)
\right]
+\nabla\cdot S=-J\cdot E,
\qquad
S=\frac1{\mu_0}E\times B.
$$

Here $S$ is the [Poynting vector](../../../electromagnetism.md#poynting-vector). Integration over $V$ gives the [Poynting theorem](../../../electromagnetism.md#poynting-theorem)

$$
\frac{dU}{dt}
=-\int_{\partial V}S\cdot n\,dS
-\int_VJ\cdot E\,d^3x.
$$

The field energy decreases through outward electromagnetic energy flux and through work done on charges.

<h3 id="15d/d">d</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/d/solution">Solution</h4>

↑ **Parent:** [D](#15d/d)

The source-free equations imply $k\cdot E_0=0$, $\omega=c|k|$, and

$$
B=\frac{k\times E_0}{\omega}\sin(k\cdot x-\omega t).
$$

Therefore

$$
S=\frac{E_0\times(k\times E_0)}{\mu_0\omega}
\sin^2(k\cdot x-\omega t)
=\epsilon_0c|E_0|^2\sin^2(k\cdot x-\omega t)\,\widehat k.
$$

It is parallel to $k$, and its period average is

$$
\langle S\rangle
=\frac12\epsilon_0c|E_0|^2\widehat k.
$$

The average electric and magnetic energy densities are equal:

$$
\langle u_E\rangle=\langle u_B\rangle
=\frac14\epsilon_0|E_0|^2.
$$

**Hence $\langle u\rangle=\epsilon_0|E_0|^2/2$ and $\langle S\rangle=c\langle u\rangle\widehat k$, as summarized by [energy density and flux of a plane electromagnetic wave](../../../electromagnetism.md#energy-density-and-flux-of-a-plane-electromagnetic-wave).**

<h3 id="15d/e">e</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/e/solution">Solution</h4>

↑ **Parent:** [E](#15d/e)

For isotropic radiation, the average power is spread over a sphere. At $r=0.10\ \mathrm m$, the [intensity of an isotropic radiator](../../../electromagnetism.md#intensity-of-an-isotropic-radiator) is

$$
\langle|S|\rangle=\frac{P}{4\pi r^2}
=\frac1{4\pi(0.10)^2}
\simeq7.96\ \mathrm{W\,m^{-2}}.
$$

Using the result of part (d),

$$
\boxed{|E_0|=\sqrt{\frac{2\langle|S|\rangle}{\epsilon_0c}}
\simeq77\ \mathrm{V\,m^{-1}}.}
$$

## 16C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16c/a">a</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/a/i">i</h4>

↑ **Parent:** [A](#16c/a)

<h5 id="16c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#16c/a/i)

Across the two vertical faces of a control rectangle, the mass fluxes are

$$
\rho u(y,t)\,\delta y
$$

with opposite signs, since $u$ is independent of $x$. There is no flux across the horizontal faces because the $y$-velocity is zero. The net mass flux is therefore zero, equivalently

$$
\boxed{\nabla\cdot u=\frac{\partial u}{\partial x}=0.}
$$

<h4 id="16c/a/ii">ii</h4>

↑ **Parent:** [A](#16c/a)

<h5 id="16c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#16c/a/ii)

The [pressure](../../../thermodynamics.md#pressure) force in the $x$-direction on a rectangle of dimensions $\delta x\times\delta y$ is

$$
-\frac{\partial p}{\partial x}\,\delta x\delta y+o(\delta x\delta y).
$$

The shear stress is $\tau_{xy}=\mu u_y$, so the net viscous force is

$$
\mu u_{yy}\,\delta x\delta y+o(\delta x\delta y).
$$

There is no convective [acceleration](../../../classical-mechanics.md#acceleration). Dividing the [momentum](../../../classical-mechanics.md#momentum) balance by the area and taking the [limit](../../../calculus.md#limit-of-a-function) gives

$$
\boxed{\rho u_t=-\frac{dp}{dx}+\mu u_{yy}}.
$$

The $y$-momentum balance gives $p_y=0$, so the [pressure](../../../thermodynamics.md#pressure) depends only on $x$.

<h3 id="16c/b">b</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/b/i">i</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#16c/b/i)

For steady flow the [momentum](../../../classical-mechanics.md#momentum) equation is

$$
\mu u''=G.
$$

Applying no slip, $u(0)=0$ and $u(h)=U$, gives the [Couette-Poiseuille flow in a thin gap](../../../viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap)

$$
\boxed{u(y)=\frac{Uy}{h}+\frac{G}{2\mu}y(y-h)}.
$$

<h4 id="16c/b/ii">ii</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#16c/b/ii)

The fluid shear stress is

$$
\tau_{xy}(y)=\mu u'(y)
=\frac{\mu U}{h}+G\left(y-\frac h2\right).
$$

The condition $\tau_{xy}(0)=0$ therefore gives

$$
\boxed{G_0=\frac{2\mu U}{h^2}}.
$$

<h4 id="16c/b/iii">iii</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#16c/b/iii)

At $G=G_0$, the linear terms cancel and

$$
u(y)=U\frac{y^2}{h^2}.
$$

The volume flux per unit width is

$$
Q=\int_0^h u(y)\,dy
=\boxed{\frac{Uh}{3}}.
$$

<h4 id="16c/b/iv">iv</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#16c/b/iv)

At the upper wall,

$$
\mu u'(h)=\frac{2\mu U}{h}.
$$

This is the shear exerted by the plate on the fluid in the positive $x$-direction. By action and reaction, the flow exerts on the top plate the stress

$$
\boxed{-\frac{2\mu U}{h}e_x}.
$$

The same result follows from a force balance on a rectangle of length $\delta x$ and full height $h$. The [pressure](../../../thermodynamics.md#pressure) force is $-G_0h\,\delta x\,e_x$, the bottom shear vanishes, and equilibrium requires the top plate to exert $G_0h\,\delta x\,e_x$ on the fluid. Thus the fluid exerts $-G_0h\,e_x=-2\mu Ue_x/h$ on the plate. These results form the [Couette-Poiseuille flow with a stress-free stationary wall](../../../viscous-fluid-flow.md#couette-poiseuille-flow-with-a-stress-free-stationary-wall).

## 17B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17b/a">a</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/a/solution">Solution</h4>

↑ **Parent:** [A](#17b/a)

The [function](../../../function.md) is not Lipschitz on $\mathbb R$. For $\varepsilon>0$,

$$
\frac{|f(\varepsilon)-f(-\varepsilon)|}{|\varepsilon-(-\varepsilon)|}
=\frac2{2\varepsilon}=\frac1\varepsilon,
$$

which is unbounded as $\varepsilon\downarrow0$.

<h3 id="17b/b">b</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/b/solution">Solution</h4>

↑ **Parent:** [B](#17b/b)

The [function](../../../function.md)

$$
y(t)=\begin{cases}
y_0-t,&0\leq t\leq y_0,\\
0,&y_0\leq t\leq T
\end{cases}
$$

is continuous, satisfies the equation away from $\widetilde t=y_0$, and has unequal one-sided [derivatives](../../../calculus.md#derivative) there.

It is unique in the stated class. While a solution is positive its [derivative](../../../calculus.md#derivative) is $-1$, so continuity forces it to follow $y_0-t$ until it first reaches zero at $t=y_0$. It cannot subsequently make a positive excursion: on any connected interval $(a,b)$ where $y>0$ and $y(a)=0$, integration of $y'=-1$ gives $y(t)=-(t-a)<0$. A negative excursion similarly contradicts $y'=1$. Hence the solution remains zero. This is the [sign-decay differential equation](../../../differential-equation.md#sign-decay-differential-equation).

<h3 id="17b/c">c</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/c/solution">Solution</h4>

↑ **Parent:** [C](#17b/c)

**Yes.** The Euler recurrence is

$$
y_{n+1}=y_n-h\operatorname{sign}(y_n).
$$

Write $y_0=mh+r$, where $m=\lfloor y_0/h\rfloor$ and $0\leq r<h$. For $n\leq m$, the numerical values agree with the exact linear descent. If $r=0$, the method reaches zero and stays there. If $0<r<h$, then

$$
y_m=r,\qquad y_{m+1}=r-h,
$$

and the recurrence thereafter alternates between $r$ and $r-h$. The exact solution is then zero, while both numerical values have magnitude at most $h$. Thus, uniformly for $0\leq n\leq N$,

$$
|y_n-y(nh)|\leq h=O(h).
$$

This is the [explicit Euler method for the sign-decay equation](../../../differential-equation.md#explicit-euler-method-for-the-sign-decay-equation).

## 18H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Independence gives

$$
\boxed{f_\mu(x_1,x_2)
=\frac1{2\pi}
\exp\left[-\frac12\left((x_1-\mu)^2+(x_2-\mu)^2\right)\right].}
$$

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

Expanding the exponent gives

$$
f_\mu(x_1,x_2)
=\frac1{2\pi}e^{-(x_1^2+x_2^2)/2}
e^{\mu(x_1+x_2)-\mu^2}.
$$

The [Fisher-Neyman factorization theorem](../../../probability-and-statistics.md#fisher-neyman-factorization-theorem) therefore shows that $T=X_1+X_2$ is sufficient.

It is also minimal sufficient. For two sample points $x,y\in\mathbb R^2$,

$$
\frac{f_\mu(x)}{f_\mu(y)}
=C(x,y)\exp\left(\mu[T(x)-T(y)]\right),
$$

where $C$ is independent of $\mu$. This ratio is independent of $\mu$ exactly when $T(x)=T(y)$. The [likelihood-ratio criterion for minimal sufficiency](../../../probability-and-statistics.md#likelihood-ratio-criterion-for-minimal-sufficiency) applies, proving the claim and the general [normal sample sum with known variance](../../../probability-and-statistics.md#normal-sample-sum-with-known-variance) result in this case.

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Writing $X_1=\mu+Z$ with $Z\sim N(0,1)$ gives

$$
\mathbb E S=\mathbb E X_1^2-1=\mu^2,
$$

so $S$ is unbiased. Its mean square error is therefore its variance. Since

$$
\mathbb E X_1^4
=\mathbb E(\mu+Z)^4
=\mu^4+6\mu^2+3,
$$

we obtain

$$
\operatorname{MSE}(S)
=\operatorname{var}(X_1^2)
=\mu^4+6\mu^2+3-(\mu^2+1)^2
=\boxed{4\mu^2+2}.
$$

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

The pair $(X_1,T)$ is jointly normal, with

$$
\mathbb EX_1=\mu,\quad \mathbb ET=2\mu,\quad
\operatorname{var}(X_1)=1,\quad
\operatorname{var}(T)=2,\quad
\operatorname{cov}(X_1,T)=1.
$$

The [conditional distribution of a bivariate normal variable](../../../probability-and-statistics.md#conditional-distribution-of-a-bivariate-normal-variable) is therefore

$$
X_1\mid T=t\sim N\left(\frac t2,\frac12\right).
$$

Equivalently, its conditional density is

$$
\boxed{f_{X_1\mid T=t}(x)=\frac1{\sqrt\pi}
\exp\left[-\left(x-\frac t2\right)^2\right].}
$$

<h3 id="18h/e">e</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/e/solution">Solution</h4>

↑ **Parent:** [E](#18h/e)

The [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) suggests conditioning $S$ on $T$. Part (d) gives

$$
\widetilde S
=\mathbb E[X_1^2-1\mid T]
=\frac12+\frac{T^2}{4}-1
=\frac{T^2}{4}-\frac12.
$$

It remains unbiased. Since $T\sim N(2\mu,2)$ and a normal variable with mean $m$ and variance $v$ satisfies $\operatorname{var}(T^2)=2v^2+4m^2v$,

$$
\operatorname{MSE}(\widetilde S)
=\frac1{16}\operatorname{var}(T^2)
=\frac1{16}(8+32\mu^2)
=\boxed{\frac12+2\mu^2}.
$$

This is strictly below $2+4\mu^2$ for every $\mu$. The calculation is recorded as the [Rao-Blackwell estimator of a squared normal mean](../../../probability-and-statistics.md#rao-blackwell-estimator-of-a-squared-normal-mean).

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

From any vertex, following the parent edge repeatedly reaches the root with positive probability $p^k$. From the root, any prescribed binary string $(b_1,\ldots,b_k)$ can be reached by following its bits, with positive probability $p_{b_1}\cdots p_{b_k}$. Thus every state communicates with every other state and the chain is irreducible.

At the root there is a self-loop of probability $p>0$, so the root has period one. All states of an irreducible chain have the same period; hence the chain is aperiodic.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

Put

$$
q=p_0+p_1=1-p.
$$

The length process $L_n=\ell(X_n)$ is a nearest-neighbour chain on the nonnegative integers: away from zero it moves up with probability $q$ and down with probability $p$, while at zero it moves up with probability $q$ and stays put with probability $p$.

Returns of the original chain to the root are exactly returns of $L_n$ to zero, so their recurrence classifications agree. The [reflected biased random walk on the nonnegative integers](../../../markov-process.md#reflected-biased-random-walk-on-the-nonnegative-integers) is transient when $q>p$, null recurrent when $q=p$, and positive recurrent when $q<p$. Since $p=1-q$, the conditions are respectively

$$
\begin{array}{c|c}
\text{classification}&\text{condition}\\ \hline
\text{transient}&p_0+p_1>\tfrac12,\\
\text{null recurrent}&p_0+p_1=\tfrac12,\\
\text{positive recurrent}&p_0+p_1<\tfrac12.
\end{array}
$$

Irreducibility transfers the classification from the root to every state.

<h3 id="19h/c">c</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/c/solution">Solution</h4>

↑ **Parent:** [C](#19h/c)

In the positive-recurrent case, let $q=p_0+p_1<p$. Detailed balance for the length chain requires

$$
\pi_kq=\pi_{k+1}p,
$$

so, with $r=q/p<1$,

$$
\pi_k=\pi_0r^k.
$$

Normalization gives $\pi_0=1-r$. The self-loop at zero makes the length chain aperiodic, so the convergence theorem for irreducible positive-recurrent aperiodic Markov chains gives

$$
\boxed{
\lim_{n\to\infty}\mathbb P(\ell(X_n)=k\mid X_0=\varnothing)
=\left(1-\frac{p_0+p_1}{p}\right)
\left(\frac{p_0+p_1}{p}\right)^k
}.
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
