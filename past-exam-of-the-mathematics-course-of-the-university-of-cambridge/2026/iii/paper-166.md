# Paper 166

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20166.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20166.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 166](paper-166.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Consider the $N+1$ [fractional parts](../../../calculus.md#fractional-part)

$$
\{0\alpha\},\{\alpha\},\ldots,\{N\alpha\}
$$

in $[0,1)$. Divide that interval into $N$ intervals of length $1/N$. By the [pigeonhole principle](../../../algebra.md#pigeonhole-principle), two fractional parts, say those indexed by $i<j$, lie in the same interval. Thus, for some [integer](../../../number-theory.md#integer) $p$,

$$
|(j-i)\alpha-p|\leq\frac1N.
$$

Set $q=j-i$. Then $1\leq q\leq N$, and division by $q$ gives the [Dirichlet approximation theorem](../../../number-theory.md#dirichlet-s-approximation-theorem)

$$
\boxed{\left|\alpha-\frac pq\right|\leq\frac1{qN}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

One Archimedean form of the [Schmidt subspace theorem](../../../number-theory.md#schmidt-subspace-theorem) is as follows. Let $L_1,\ldots,L_n$ be linearly independent [linear forms](../../../linear-algebra.md#linear-functional) in $n$ variables with algebraic coefficients. For every $\varepsilon>0$, all nonzero $\mathbf x\in\mathbb Z^n$ satisfying

$$
\prod_{i=1}^n|L_i(\mathbf x)|
<\|\mathbf x\|^{-\varepsilon}
$$

belong to a finite union of proper rational [linear subspaces](../../../vector-space.md#vector-subspace) of $\mathbb Q^n$.

We will also use its finite-place form: if $S$ is a finite set of places containing the Archimedean ones and, for each $v\in S$, the forms $L_{1,v},\ldots,L_{n,v}$ are independent, then the integer solutions of

$$
\prod_{v\in S}\prod_{i=1}^n|L_{i,v}(\mathbf x)|_v
<H(\mathbf x)^{-\varepsilon}
$$

lie in finitely many proper rational subspaces. The absolute values are normalized so that the [product formula](../../../algebraic-number-theory.md#product-formula) holds.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Roth theorem](../../../number-theory.md#roth-s-theorem) states that if $\alpha$ is a real algebraic irrational number, then for every $\varepsilon>0$ there are only finitely many reduced fractions $p/q$ satisfying

$$
\left|\alpha-\frac pq\right|<q^{-2-\varepsilon}.
$$

To derive this from the [Schmidt subspace theorem](../../../number-theory.md#schmidt-subspace-theorem), take

$$
L_1(X,Y)=X-\alpha Y,
\qquad
L_2(X,Y)=Y.
$$

These forms are linearly independent. For a solution $(p,q)$ with $q$ large, $|p|\asymp q$, so $H(p,q)\asymp q$, while

$$
|L_1(p,q)L_2(p,q)|
=|p-\alpha q|q
=q^2\left|\alpha-\frac pq\right|
<q^{-\varepsilon}.
$$

After slightly decreasing $\varepsilon$, the [Schmidt subspace theorem](../../../number-theory.md#schmidt-subspace-theorem) puts all such primitive vectors $(p,q)$ in finitely many rational lines. Each rational line contains only the two opposite primitive integer vectors $\pm(p,q)$, and these determine the same fraction. Hence only finitely many fractions occur.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Fix a finite set $S$ of [primes](../../../number-theory.md#prime-number). We prove that only finitely many denominators $q_n$ can be [S-smooth number](../../../number-theory.md#s-smooth-number). This is the standard finite-place corollary of the [Schmidt subspace theorem](../../../number-theory.md#schmidt-subspace-theorem) for [best approximations of the first kind](../../../number-theory.md#best-rational-approximation); the reduction is recalled here because the target $\alpha$ need not be algebraic.

Apply the [Dirichlet approximation theorem](../../../number-theory.md#dirichlet-s-approximation-theorem) at each cutoff between two successive record denominators. Its approximant can be replaced by the last record without increasing the error. Apply the finite-place [Schmidt subspace theorem](../../../number-theory.md#schmidt-subspace-theorem) to the resulting pairs of primitive vectors, using $X-\alpha Y,Y$ at the real place only after eliminating $\alpha$ between two successive pairs, and $X,Y$ at every place belonging to $S$. The factors

$$
\prod_{\ell\in S}|q_n|_\ell=q_n^{-1}
$$

for an $S$-smooth denominator supply the required height saving. If infinitely many such records existed, one fixed rational subspace would contain infinitely many of the paired vectors. Eliminating its rational linear relation has two possible outcomes: either all sufficiently late records represent one rational number, which contradicts the irrationality of $\alpha$, or $\alpha$ is algebraic and, for some $\eta>0$, infinitely many of the records satisfy

$$
\left|\alpha-\frac{p_n}{q_n}\right|<q_n^{-2-\eta}.
$$

The latter alternative contradicts the [Roth theorem](../../../number-theory.md#roth-s-theorem). Thus only finitely many $q_n$ are $S$-smooth.

If the [largest prime factor](../../../number-theory.md#largest-prime-factor) of $q_n$ did not tend to infinity, some bound $B$ would contain the largest prime factor for infinitely many $n$. Taking $S$ to be the finite set of primes at most $B$ would make those denominators $S$-smooth, contrary to the preceding conclusion. Therefore $P^+(q_n)\to\infty$.

## 2

↑ **Parent:** [Paper 166](paper-166.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

If

$$
P(X)=a_d\prod_{i=1}^d(X-\alpha_i),
$$

its [Mahler measure](../../../algebraic-number-theory.md#mahler-measure) is

$$
M(P)=|a_d|\prod_{i=1}^d\max(1,|\alpha_i|).
$$

If $f_\alpha\in\mathbb Z[X]$ is the primitive minimal polynomial of an algebraic number $\alpha$ and $d=\deg f_\alpha$, the [height-Mahler measure formula](../../../algebraic-number-theory.md#height-mahler-measure-formula) is

$$
\boxed{H(\alpha)^d=M(f_\alpha).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose a [number field](../../../algebraic-number-theory.md#number-field) $L$ containing $\alpha_1,\ldots,\alpha_k$. At every place $v$ of $L$, put

$$
A_v=\prod_{j=1}^k\max(1,|\alpha_j|_v)^{n_j}.
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\max\{|P(\boldsymbol\alpha)|_v,|Q(\boldsymbol\alpha)|_v\}
\leq c_vA_v,
$$

where $c_v=1$ at every non-Archimedean place because the coefficients are [integers](../../../number-theory.md#integer), while at an Archimedean place one may take

$$
c_v=\max\{\mathcal L(P),\mathcal L(Q)\}.
$$

Raise these inequalities to the local weights and multiply over all places. The definition of the [Absolute multiplicative Weil height](../../../algebraic-number-theory.md#absolute-multiplicative-weil-height) and the [product formula](../../../algebraic-number-theory.md#product-formula) then give

$$
H\left(\frac{P(\alpha_1,\ldots,\alpha_k)}
{Q(\alpha_1,\ldots,\alpha_k)}\right)
\leq
\max\{\mathcal L(P),\mathcal L(Q)\}
\prod_{j=1}^kH(\alpha_j)^{n_j}.
$$

This is the [height bound for a polynomial evaluation](../../../algebraic-number-theory.md#height-bound-for-a-polynomial-evaluation).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take distinct $x,y\in A_n$. Their difference has the form

$$
x-y=P(\alpha),
$$

where $P\in\mathbb Z[X]$ has degree at most $n-1$ and [polynomial length](../../../polynomial.md#polynomial-length) at most $nh$. By the [height bound for a polynomial evaluation](../../../algebraic-number-theory.md#height-bound-for-a-polynomial-evaluation),

$$
H(x-y)\leq nh\,H(\alpha)^{n-1}.
$$

The algebraic number $x-y$ is nonzero and has degree at most $d$, so the [Liouville height inequality](../../../algebraic-number-theory.md#liouville-height-inequality) gives the separation

$$
|x-y|
\geq(nh)^{-d}H(\alpha)^{-d(n-1)}.
$$

All elements of $A_n$ lie in an interval of length at most

$$
\frac h{1-\alpha}.
$$

Since $H(1-\alpha)\leq2H(\alpha)$, another application of the [Liouville height inequality](../../../algebraic-number-theory.md#liouville-height-inequality) gives

$$
\frac1{1-\alpha}\leq(2H(\alpha))^d.
$$

The number of points in an interval is at most one plus its length divided by their minimum separation. Consequently

$$
|A_n|
\leq
2^dh(nh)^dH(\alpha)^{dn}+1
\leq
(2hn)^{d+1}H(\alpha)^{dn}+1.
$$

**Thus the requested statement holds, for example, with the absolute constant $C=2$.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Suppose, for a contradiction, that suitable nonzero polynomials vanish at both $\alpha^k$ and $\alpha^{k+1}$. If $P(\gamma)=0$, then the primitive [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $f_\gamma$ divides $P$. The multiplicativity of [Mahler measure](../../../algebraic-number-theory.md#mahler-measure) and the [Mahler measure bounded by polynomial length](../../../algebraic-number-theory.md#mahler-measure-bounded-by-polynomial-length) give

$$
H(\gamma)^{[\mathbb Q(\gamma):\mathbb Q]}
=M(f_\gamma)
\leq M(P)
\leq\mathcal L(P)
<nh.
$$

If $[\mathbb Q(\alpha^k):\mathbb Q]=d$, then, using $H(\alpha^k)=H(\alpha)^k$, this inequality contradicts $H(\alpha)^{kd}>nh$. Hence $\mathbb Q(\alpha^k)$ is a proper intermediate field of $\mathbb Q(\alpha)/\mathbb Q$. Its degree divides the prime $d$ by the [tower law](../../../algebra.md#tower-law), so $\alpha^k\in\mathbb Q$. Applying the same argument to $\alpha^{k+1}$ is even stronger and gives $\alpha^{k+1}\in\mathbb Q$. Since $\alpha\ne0$,

$$
\alpha=\frac{\alpha^{k+1}}{\alpha^k}\in\mathbb Q,
$$

contrary to $d\geq2$. At least one of the two proposed values of $\beta$ therefore has no such polynomial relation.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Write $H=H(\alpha)$. Since $\alpha$ has degree at least two and lies in $(0,1)$, $H>1$. Put

$$
x=\frac{\log(nh)}{d\log H}>1,
\qquad
k=\lfloor x\rfloor+1.
$$

Then $H^{kd}>nh$ and

$$
k+1\leq x+2\leq3x.
$$

Let

$$
m=\left\lceil\frac n{k+1}\right\rceil.
$$

Part (d), applied with $m$ in place of its polynomial-degree parameter, supplies $\ell\in\{k,k+1\}$ such that no nonzero integer polynomial of degree at most $m-1$ and with coefficients of absolute value less than $h$ vanishes at $\beta=\alpha^\ell$.

It follows that the $h^m$ sums

$$
\sum_{j=0}^{m-1}a_j\beta^j,
\qquad 0\leq a_j<h,
$$

are distinct. Since

$$
(m-1)\ell\leq(m-1)(k+1)\leq n-1,
$$

they form a subset of $A_n$. Hence

$$
|A_n|\geq h^m
\geq h^{\,n/(k+1)}
\geq h^{\,dn\log H/(3\log(nh))}
=H^{\,dn\log h/(3\log(nh))},
$$

as required.

## 3

↑ **Parent:** [Paper 166](paper-166.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\beta\in K$, the nonzero algebraic number $\gamma=\alpha-\beta$ has degree at most

$$
[\mathbb Q(\alpha,\beta):\mathbb Q]\leq3\cdot2=6.
$$

The basic height inequality gives

$$
H(\gamma)\leq2H(\alpha)H(\beta).
$$

The [Liouville height inequality](../../../algebraic-number-theory.md#liouville-height-inequality) therefore yields

$$
|\alpha-\beta|
\geq H(\gamma)^{-6}
\geq(2H(\alpha))^{-6}H(\beta)^{-6}.
$$

Thus one may take the explicit constant

$$
\boxed{c=(2H(\alpha))^{-6}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A suitable theorem is the [Baker lower bound for a homogeneous linear form in logarithms](../../../number-theory.md#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms). Let $\alpha_1,\ldots,\alpha_n$ be nonzero algebraic numbers with chosen logarithms and let

$$
\Lambda=b_1\log\alpha_1+\cdots+b_n\log\alpha_n,
\qquad b_i\in\mathbb Z.
$$

Choose $A_i\geq3$ to bound the degree-normalized [Absolute logarithmic Weil height](../../../algebraic-number-theory.md#absolute-logarithmic-weil-height) of $\alpha_i$ and $|\log\alpha_i|$, and put $B=\max(3,|b_1|,\ldots,|b_n|)$. If $\Lambda\ne0$, then

$$
\log|\Lambda|
>-C(\log A_1)\cdots(\log A_n)\log B,
$$

where $C$ is an effectively computable constant depending only on $n$ and the degree of the number field generated by the $\alpha_i$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $f$ be the monic cubic minimal polynomial of the [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer) $\alpha$, let $\alpha_1=\alpha,\alpha_2,\alpha_3$ be its conjugates, and let $\beta_1=\beta,\beta_2$ be the two conjugates of a nonrational $\beta\in\mathcal O_K$. Because the degrees three and two are coprime, the fields are [linearly disjoint](../../../algebra.md#linear-disjointness), and

$$
m=N_{\mathbb Q(\alpha)K/\mathbb Q}(\alpha-\beta)
=\prod_{i=1}^3\prod_{j=1}^2(\alpha_i-\beta_j)
$$

is a nonzero [integer](../../../number-theory.md#integer).

Assume

$$
|\alpha-\beta|\leq H(\beta)^{-(6-\varepsilon)}.
$$

For large $H(\beta)$ this makes $\beta_1$ bounded. Since $\beta$ is a quadratic [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer), the [height-Mahler measure formula](../../../algebraic-number-theory.md#height-mahler-measure-formula) gives

$$
H(\beta)^2=\max(1,|\beta_1|)\max(1,|\beta_2|),
$$

and therefore $|\beta_2|\asymp H(\beta)^2$. The two remaining factors with $j=1$ are bounded, while the three factors with $j=2$ are $O(|\beta_2|)$. Consequently

$$
1\leq|m|
\leq C_{\alpha,K}|\alpha-\beta|\,|\beta_2|^3
\leq C_{\alpha,K}H(\beta)^\varepsilon.
$$

We now use the standard effective [norm form](../../../algebraic-number-theory.md#norm-form) consequence of Part (b). For

$$
L=\mathbb Q(\alpha)K,
\qquad
V=\operatorname{span}_{\mathbb Q}\{1,\alpha,\omega\},
$$

where $1,\omega$ is an integral basis of $K$, the [effective norm-form height estimate](../../../number-theory.md#effective-norm-form-height-estimate) supplies effective constants $A,C>0$, depending only on $\alpha$ and $K$, such that

$$
H(z)\leq C|N_{L/\mathbb Q}(z)|^A
$$

for every nonzero $z\in V\cap\mathcal O_L$. Its proof factors $(z)$, balances a generator using the [Dirichlet unit theorem](../../../algebraic-number-theory.md#dirichlet-s-unit-theorem), and applies the [Baker lower bound for a homogeneous linear form in logarithms](../../../number-theory.md#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms) to the linear relations defining $V$; the coprime degrees $3$ and $2$ exclude a unit-family degeneracy.

Apply this estimate to $z=\alpha-\beta$. Since $\beta=\alpha-z$, the height inequalities imply $H(\beta)\leq2H(\alpha)H(z)$. Hence

$$
H(\beta)
\leq C'|m|^A
\leq C''H(\beta)^{A\varepsilon}.
$$

Choose the effective value $\varepsilon=1/(2A)$. The last inequality bounds $H(\beta)$ effectively. The rational integers $\beta\in\mathbb Z$ are already covered by the stronger degree-three [Liouville approximation theorem](../../../number-theory.md#liouville-approximation-theorem), and the [Northcott theorem](../../../algebraic-number-theory.md#northcott-theorem) leaves only finitely many remaining quadratic integers of bounded height. Taking the minimum of

$$
|\alpha-\beta|H(\beta)^{6-\varepsilon}
$$

over this effective finite set gives an effective $c>0$ and proves

$$
|\alpha-\beta|\geq cH(\beta)^{-(6-\varepsilon)}
$$

for every $\beta\in\mathcal O_K$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
