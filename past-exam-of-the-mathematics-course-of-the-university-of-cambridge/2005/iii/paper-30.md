# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper30.pdf)

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

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $X=1+T$ and $Y=X^p-1$, so that $\phi(f)=f(Y)$. The essential integrality statement for the [Frobenius substitution on cyclotomic power series](../../../algebraic-number-theory.md#frobenius-substitution-on-cyclotomic-power-series) is the decomposition into a [finite free module](../../../module-theory.md#finite-free-module):

$$
R=\bigoplus_{i=0}^{p-1}X^i\phi(R).
$$

To prove it, reduce modulo $p$. Since $Y\equiv T^p$, grouping the coefficients of a [formal power series](../../../commutative-algebra.md#formal-power-series) according to their exponents modulo $p$ gives the unique expression $\sum_{j=0}^{p-1}T^jh_j(T^p)$. The change from $1,T,\ldots,T^{p-1}$ to $1,X,\ldots,X^{p-1}$ is a triangular [matrix](../../../vector-space.md#matrix) with diagonal entries $1$, so this is also a [basis](../../../vector-space.md#basis) over $\mathbb F_p[[T^p]]$. Lift these $p$ coefficient series to $R$, subtract their contribution from $f$, divide the remaining error by $p$, and repeat. The sums of the successive lifts converge in the finer of the [topologies on integral formal power series](../../../commutative-algebra.md#topologies-on-integral-formal-power-series), because $R$ is complete in that topology. This proves existence of the decomposition over $R$. A relation among its summands reduces to the zero relation modulo $p$, forcing each coefficient series to be divisible by $p$. Repetition forces divisibility by every power of $p$, hence every coefficient series is zero. This proves uniqueness and, in particular, [injectivity](../../../algebra.md#injective-function) of $\phi$.

For $f=\sum_{i=0}^{p-1}X^i\phi(f_i)$, define

$$
\boxed{S(f)=f_0.}
$$

This is a $\mathbb Z_p$-[linear map](../../../vector-space.md#linear-map). To calculate the average over [roots of unity](../../../algebra.md#root-of-unity), work over $\mathcal O=\mathbb Z_p[\zeta_p]$. The substitutions $T\mapsto\zeta X-1$ are legitimate: their constant terms are topologically nilpotent, so the defining coefficient sums converge in $\mathcal O$. Since $(\zeta X)^p=X^p$, each $\phi(f_i)$ is unchanged by the substitution. The sums of the powers of the [roots of unity](../../../algebra.md#root-of-unity) are $p$ for $i=0$ and zero for $1\leq i<p$. Consequently

$$
\sum_{\zeta\in\mu_p}f(\zeta X-1)=p\phi(f_0).
$$

Thus the average is integral and belongs to $\phi(R)$, and the constructed [Coleman trace operator](../../../algebraic-number-theory.md#coleman-trace-operator) has the required property. [Injectivity](../../../algebra.md#injective-function) of $\phi$ forces uniqueness of any map satisfying that property. Finally, the decomposition of $\phi(g)$ has $f_0=g$ and all other coefficients zero, giving **$S\circ\phi=\mathrm{id}_R$**.

We will also use the [trace](../../../linear-algebra.md#matrix-trace) of multiplication by $h$ on this [finite free module](../../../module-theory.md#finite-free-module). After extending scalars to split the conjugates, that [trace](../../../linear-algebra.md#matrix-trace) is the sum just computed. Hence

$$
\operatorname{Tr}_{R/\phi(R)}(h)=p\phi(S(h)).
$$

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $M_f$ be the [matrix](../../../vector-space.md#matrix) of multiplication by $f$ in the [basis](../../../vector-space.md#basis) from Question 1. Define the [Coleman norm operator](../../../algebraic-number-theory.md#coleman-norm-operator) by the [norm for a finite free ring extension](../../../commutative-algebra.md#norm-for-a-finite-free-ring-extension):

$$
\boxed{\phi(Nf)=\det(M_f).}
$$

The entries lie in $\phi(R)$, and $\phi:R\to\phi(R)$ is an [isomorphism](../../../algebra.md#isomorphism), so this determines $Nf$ uniquely. If $f$ is a [unit](../../../algebra.md#unit-in-a-ring), $M_f$ is invertible and its [determinant](../../../linear-algebra.md#determinant) is a [unit](../../../algebra.md#unit-in-a-ring). Also $M_{fg}=M_fM_g$, giving $N(fg)=Nf\,Ng$. Splitting the conjugates, or diagonalizing multiplication after adjoining the [roots of unity](../../../algebra.md#root-of-unity) and inverting $p$, gives the equivalent formula

$$
\phi(Nf)(T)=\prod_{\zeta\in\mu_p}f(\zeta(1+T)-1).
$$

In particular, this definition has the required target $R^\times$, rather than merely a [ring](../../../commutative-algebra.md#ring) with extra [roots of unity](../../../algebra.md#root-of-unity) in its coefficients.

For the requested [ring congruence](../../../commutative-algebra.md#congruence-modulo-an-ideal), observe that the reduction of $\phi$ is the injective map $\overline g(T)\mapsto\overline g(T^p)$. If $\phi(g)\in p^kR$, its reduction first gives $g=pg_1$. Then $\phi(g_1)\in p^{k-1}R$; repeat to obtain $g\in p^kR$. Applying this to $g=f-1$ proves

$$
\boxed{\phi(f)\equiv1\pmod{p^kR}\ \Longrightarrow\ f\equiv1\pmod{p^kR}.}
$$

This [congruence reflection for Frobenius substitution](../../../algebraic-number-theory.md#congruence-reflection-for-frobenius-substitution) is valid for all $f\in R$, without assuming $f$ is a [unit](../../../algebra.md#unit-in-a-ring).

A further property needed for the fixed points is [Coleman norm contraction](../../../algebraic-number-theory.md#coleman-norm-contraction). If $g=1+p^kh$ with $k\geq1$, expand the [determinant](../../../linear-algebra.md#determinant):

$$
\phi(Ng)=\det(I+p^kM_h)=1+p^k\operatorname{Tr}(M_h)+\sum_{j=2}^{p}p^{kj}e_j(M_h).
$$

Here $e_j(M_h)\in\phi(R)$ is the coefficient of degree $j$ in $\det(I+tM_h)$. The [trace](../../../linear-algebra.md#matrix-trace) formula from Question 1 makes the linear term divisible by $p^{k+1}$; every later term is divisible by $p^{2k}$ and $2k\geq k+1$. Reflecting the resulting [ring congruence](../../../commutative-algebra.md#congruence-modulo-an-ideal) through $\phi$ gives

$$
N(1+p^kR)\subseteq1+p^{k+1}R.
$$

If $Nf=f$ and $f\in1+pR$, iteration gives $f\in1+p^kR$ for every $k$. Since $\bigcap_k p^kR=0$, **$f=1$**.

To identify all fixed points, we also need $Nf\equiv f\pmod{pR}$ for every [unit](../../../algebra.md#unit-in-a-ring) $f$. In characteristic $p$, the extension $\mathbb F_p[[T]]/\mathbb F_p[[T^p]]$ has degree $p$ and its [norm for a finite free ring extension](../../../commutative-algebra.md#norm-for-a-finite-free-ring-extension) is $\overline f\mapsto\overline f^{\,p}$. Indeed, after passing to [fraction fields](../../../commutative-algebra.md#field-of-fractions) it is a [purely inseparable field extension](../../../galois-theory.md#purely-inseparable-extension) of degree $p$, so multiplication has only the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\overline f$, with multiplicity $p$, after splitting. Its [determinant](../../../linear-algebra.md#determinant) is $\overline f^{\,p}$. Therefore

$$
\overline{\phi(Nf)}=\overline f^{\,p}=\overline{\phi(f)},
$$

and [congruence reflection for Frobenius substitution](../../../algebraic-number-theory.md#congruence-reflection-for-frobenius-substitution) gives $Nf\equiv f\pmod{pR}$.

Now choose any lift $f_0\in R^\times$ of a given $a\in A^\times$ and put $f_n=N^nf_0$. Multiplicativity gives

$$
\frac{f_{n+1}}{f_n}=N^n\left(\frac{Nf_0}{f_0}\right)\in1+p^{n+1}R.
$$

Thus $(f_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) for the finer of the [topologies on integral formal power series](../../../commutative-algebra.md#topologies-on-integral-formal-power-series) and converges to a [unit](../../../algebra.md#unit-in-a-ring) $w(a)$ reducing to $a$. The [Coleman norm operator](../../../algebraic-number-theory.md#coleman-norm-operator) is continuous: multiplication matrices and their [determinants](../../../linear-algebra.md#determinant) are continuous, and the finite-free coordinate decomposition and its inverse preserve the $p$-adic filtration defining the finer of the [topologies on integral formal power series](../../../commutative-algebra.md#topologies-on-integral-formal-power-series). Hence $Nw(a)=w(a)$. If two fixed [units](../../../algebra.md#unit-in-a-ring) reduce to $a$, their quotient is fixed and belongs to $1+pR$, so it is $1$ by the preceding argument. This proves uniqueness, independence of the initial lift, and multiplicativity of the [Coleman norm-fixed lift](../../../algebraic-number-theory.md#coleman-norm-fixed-lift). In particular,

$$
\boxed{W\xrightarrow[\text{reduction}]{\ \sim\ }A^\times,\qquad a\longmapsto w(a)=\lim_{n\to\infty}N^nf_0\text{ in the inverse direction}.}
$$

Every [unit](../../../algebra.md#unit-in-a-ring) $f\in R$ consequently has a unique factorization $f=w(\overline f)v$ with $v\in1+pR$, giving the [canonical Coleman decomposition of power-series units](../../../algebraic-number-theory.md#canonical-coleman-decomposition-of-power-series-units):

$$
\boxed{R^\times\simeq W\times(1+pR),\qquad f\longmapsto\left(w(\overline f),\frac{f}{w(\overline f)}\right).}
$$

**The final assertion as printed is false.** The original PDF identifies a [ring](../../../commutative-algebra.md#ring) with a product of [unit groups](../../../algebra.md#unit-group). With multiplication, $A$ has a zero and is not a [group](../../../group.md). With addition, it has exponent $p$, whereas $W\times A^\times$ has a nonidentity element of order $2$: $-1\in W$ because $p$ is odd and $N(-1)=(-1)^p=-1$. Thus neither interpretation makes the printed assertion true. The two boxed isomorphisms above are the valid natural conclusions; they do not require guessing which symbols the author intended to replace.

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [profinite abelian group](../../../topological-group.md#profinite-abelian-group) $G$, its [Iwasawa algebra](../../../associative-algebra.md#iwasawa-algebra) is the completed [group algebra](../../../associative-algebra.md#group-algebra)

$$
\boxed{\Lambda(G)=\varprojlim_U\mathbb Z_p[G/U]=\varprojlim_{U,r}(\mathbb Z/p^r\mathbb Z)[G/U],}
$$

where $U$ runs over open [subgroups](../../../group.md#subgroup). The transition map sums the coefficients over the fibers of $G/V\to G/U$ when $V\subset U$. Consequently an element gives compatible values $\mu(gU)\in\mathbb Z_p$ on [cosets](../../../group-theory.md#coset), equivalently a finitely additive $\mathbb Z_p$-valued [p-adic measure](../../../measure-theory.md#p-adic-measure) on the [clopen sets](../../../topology.md#clopen-set) of $G$. Conversely these values specify every finite-quotient coefficient. Integration of a [continuous function](../../../calculus.md#continuous-function) with values in $\mathbb Z_p$ is obtained by uniform approximation by locally constant functions; the integrals converge because all measure values have $p$-adic absolute value at most $1$. Multiplication in the [Iwasawa algebra](../../../associative-algebra.md#iwasawa-algebra) becomes [convolution of p-adic measures](../../../measure-theory.md#convolution-of-p-adic-measures). This is its [measure realization of an Iwasawa algebra](../../../associative-algebra.md#measure-realization-of-an-iwasawa-algebra).

The [Mahler theorem](../../../arithmetic.md#mahler-s-theorem) states that each [continuous function](../../../calculus.md#continuous-function) $g:\mathbb Z_p\to\mathbb Z_p$ has the unique expansion converging in the sense of [uniform convergence](../../../real-analysis.md#uniform-convergence)

$$
g(x)=\sum_{n\geq0}b_n\binom{x}{n},\qquad b_n\in\mathbb Z_p,\quad b_n\longrightarrow0.
$$

Its [Mahler coefficients](../../../arithmetic.md#mahler-coefficient) are

$$
b_n=\Delta^ng(0)=\sum_{j=0}^{n}(-1)^{n-j}\binom njg(j),
$$

and $\|g\|_\infty=\sup_n|b_n|_p$. The same assertion holds for [continuous functions](../../../calculus.md#continuous-function) with values in $\mathbb Q_p$ with coefficients in $\mathbb Q_p$.

Given $f(T)=\sum_{n\geq0}a_nT^n\in R$, define the [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional)

$$
L_f(g)=\sum_{n\geq0}a_nb_n.
$$

The sum converges because $a_n\in\mathbb Z_p$ and $b_n\to0$. Its values on [indicator functions](../../../measure-theory.md#indicator-function) of [clopen sets](../../../topology.md#clopen-set) give a [p-adic measure](../../../measure-theory.md#p-adic-measure), denoted $\lambda(f)$, with

$$
\int_{\mathbb Z_p}\binom{x}{n}\,d\lambda(f)=a_n.
$$

Conversely, a [p-adic measure](../../../measure-theory.md#p-adic-measure) determines these coefficients $a_n\in\mathbb Z_p$, and continuity allows termwise integration of every [Mahler expansion](../../../arithmetic.md#mahler-s-theorem). Thus the inverse is

$$
\mu\longmapsto\sum_{n\geq0}\left(\int\binom{x}{n}\,d\mu\right)T^n,
$$

which is the [Amice transform](../../../measure-theory.md#amice-transform). These two constructions are inverse, proving the **canonical bijection $\lambda:R\simeq\Lambda(\mathbb Z_p)$**. In fact it is an [isomorphism](../../../algebra.md#isomorphism) of [rings](../../../commutative-algebra.md#ring): the identity $\binom{x+y}{n}=\sum_{i+j=n}\binom{x}{i}\binom{y}{j}$ identifies [convolution of p-adic measures](../../../measure-theory.md#convolution-of-p-adic-measures) with multiplication of [formal power series](../../../commutative-algebra.md#formal-power-series). For example, $\lambda(1)=\delta_0$ and $\lambda(1+T)=\delta_1$, where $\delta_a$ is the [Dirac measure](../../../measure-theory.md#dirac-measure) at $a$.

For the moment identity, let $\left\{{k\atop n}\right\}$ denote a [Stirling number of the second kind](../../../combinatorics.md#stirling-numbers-of-the-second-kind). The finite [polynomial identity](../../../polynomial.md#polynomial-identity)

$$
x^k=\sum_{n=0}^{k}n!\left\{{k\atop n}\right\}\binom{x}{n}
$$

gives $\int x^k\,d\lambda(f)=\sum_{n=0}^{k}a_n n!\left\{{k\atop n}\right\}$. On the other hand, $D=(1+T)d/dT$ satisfies $D^k(1+T)^x=x^k(1+T)^x$ for every nonnegative integer $x$. Expanding $(1+T)^x$ and evaluating at $T=0$ yields

$$
x^k=\sum_{n=0}^{k}\binom{x}{n}(D^kT^n)(0).
$$

Comparison in the [basis](../../../vector-space.md#basis) of binomial [polynomials](../../../polynomial.md) gives $(D^kT^n)(0)=n!\left\{{k\atop n}\right\}$. Terms with $n>k$ have zero constant term after at most $k$ differentiations, so no infinite-series interchange is needed. Therefore

$$
\boxed{\int_{\mathbb Z_p}x^k\,d\lambda(f)=(D^kf)(0)\qquad(k\geq0).}
$$

The case $k=0$ says that the total mass is $f(0)$.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The preceding constructions lead to the [Iwasawa theorem on local cyclotomic units](../../../algebraic-number-theory.md#iwasawa-theorem-on-local-cyclotomic-units). Its significance is that an explicitly calculated [local unit](../../../algebra.md#local-unit-of-a-local-field) quotient is governed by a [p-adic L-function](../../../analytic-number-theory.md#p-adic-l-function); [class field theory](../../../algebraic-number-theory.md#class-field-theory) then suggests that the same analytic object should govern global arithmetic. The latter prediction is the [Iwasawa main conjecture](../../../algebraic-number-theory.md#main-conjecture-of-iwasawa-theory), rather than a consequence of the local calculation alone.

Fix compatible [roots of unity](../../../algebra.md#root-of-unity) $\zeta_{p^n}$ and put $K_n=\mathbb Q_p(\zeta_{p^n})$, $\pi_n=\zeta_{p^n}-1$. Let $V_\infty$ be the norm limit of the local [principal units](../../../arithmetic.md#principal-unit). Take its even part under [complex conjugation](../../../complex-analysis.md#complex-conjugation) to obtain $U_\infty^1$, the local principal-unit limit in the real tower. Let $C_\infty^1$ be the closed [subgroup](../../../group.md#subgroup) generated by norm-compatible real [cyclotomic units](../../../galois-theory.md#cyclotomic-unit), with their finite-order residue factors removed. Write

$$
G=\mathbb Z_p^\times/\{\pm1\},\qquad \Lambda_G=\mathbb Z_p[[G]],\qquad I(G)=\ker(\Lambda_G\longrightarrow\mathbb Z_p).
$$

Here the last map is augmentation. Normalize the [p-adic zeta pseudomeasure](../../../analytic-number-theory.md#p-adic-zeta-pseudomeasure) $\zeta_p$ by

$$
\int_Gx^k\,d\zeta_p=(1-p^{k-1})\zeta(1-k)=-(1-p^{k-1})\frac{B_k}{k}\qquad(k\geq2\text{ even}).
$$

The expression $x^k$ is well defined on $G$ for even $k$. A pseudomeasure lies in the total fraction [ring](../../../commutative-algebra.md#ring) of the [Iwasawa algebra](../../../associative-algebra.md#iwasawa-algebra); the pole on its trivial finite-character component is removed by the [augmentation ideal](../../../commutative-algebra.md#augmentation-ideal), so $I(G)\zeta_p\subset\Lambda_G$. In this normalization the local theorem is

$$
\boxed{U_\infty^1/C_\infty^1\simeq\Lambda_G/(I(G)\zeta_p).}
$$

The following steps outline its proof and explain where the earlier questions enter.

First encode [local units](../../../algebra.md#local-unit-of-a-local-field) by [Coleman power series](../../../algebraic-number-theory.md#coleman-power-series). Evaluation at $\pi_n$ is surjective from $R$ to $\mathcal O_{K_n}$, and the product defining the [Coleman norm operator](../../../algebraic-number-theory.md#coleman-norm-operator) gives

$$
(Nf)(\pi_{n-1})=N_{K_n/K_{n-1}}(f(\pi_n))\qquad(n\geq2).
$$

Thus norm-fixed series give [norm-compatible sequences of local units](../../../algebraic-number-theory.md#norm-compatible-sequence-of-local-units). Conversely, lift $u_m$ from such a sequence to $f^{(m)}\in R^\times$ and take $g_m=N^{m-r_m}f^{(m)}$, where $r_m=\lfloor m/2\rfloor$. This has $g_m(\pi_{r_m})=u_{r_m}$. The estimates in Question 2 give $Ng_m/g_m\in1+p^{m-r_m+1}R$. Consequently for fixed $n\leq r_m$, the series $N^{r_m-n}g_m$ differs from $g_m$ modulo $p^{m-r_m+1}$ and its value at $\pi_n$ is $u_n$. The [compactness](../../../topology.md#compact-space) of $R$ in the coarser of the [topologies on integral formal power series](../../../commutative-algebra.md#topologies-on-integral-formal-power-series) supplies a convergent subsequence. Continuity of the [Coleman norm operator](../../../algebraic-number-theory.md#coleman-norm-operator) and of evaluation shows that its limit is norm-fixed and takes every value $u_n$. It is a [unit](../../../algebra.md#unit-in-a-ring) because the original [principal units](../../../arithmetic.md#principal-unit) have residue $1$. Uniqueness follows from the [Weierstrass preparation theorem](../../../arithmetic.md#weierstrass-preparation-theorem): a nonzero series in $R$ has only finitely many zeros in the open unit disk, whereas the distinct $\pi_n$ give infinitely many interpolation points. This constructs the [Coleman power series](../../../algebraic-number-theory.md#coleman-power-series) $f_u$.

Next turn its multiplicative information into an integral [p-adic measure](../../../measure-theory.md#p-adic-measure). For a norm-fixed [unit](../../../algebra.md#unit-in-a-ring) $f$, use the [Frobenius-corrected logarithm](../../../algebraic-number-theory.md#frobenius-corrected-logarithm)

$$
\mathcal L(f)=\frac1p\log\left(\frac{f^p}{\phi(f)}\right).
$$

The ratio belongs to $1+pR$ by reduction modulo $p$, and the logarithm divided by $p$ is integral because $p$ is odd. Equivalently $\mathcal L(f)=(1-\phi/p)\log f$, interpreting the constant coefficient with the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) on [units](../../../algebra.md#unit-in-a-ring). The averaging identity for the logarithm is understood on the open $p$-adic unit disk, where the translated logarithmic series converge; the corrected result itself lies in $R$. The logarithmic product formula and Question 1 give

$$
S\log f=\frac1p\log(Nf),\qquad S\mathcal L(f)=\frac1p\log(Nf/f)=0.
$$

Under the [Amice transform](../../../measure-theory.md#amice-transform), the root-of-unity average projects a [p-adic measure](../../../measure-theory.md#p-adic-measure) onto its restriction to $p\mathbb Z_p$: the averaged factor $(1+T)^x$ survives exactly for $x\in p\mathbb Z_p$. Consequently $S\mathcal L(f)=0$ says that $\lambda(\mathcal L(f))$ is supported on $\mathbb Z_p^\times$. This gives a [Galois group](../../../galois-theory.md#galois-group)-equivariant homomorphism from local [principal units](../../../arithmetic.md#principal-unit) to the [Iwasawa algebra](../../../associative-algebra.md#iwasawa-algebra) of $\mathbb Z_p^\times$.

The integral lifting step in this proof is the [Coleman unit-measure exact sequence](../../../algebraic-number-theory.md#coleman-unit-measure-exact-sequence)

$$
0\longrightarrow\mathbb Z_p(1)\longrightarrow V_\infty\xrightarrow{\mathrm{Col}}\mathbb Z_p[[\mathbb Z_p^\times]]\xrightarrow{m_1}\mathbb Z_p(1)\longrightarrow0,\qquad m_1(\mu)=\int x\,d\mu.
$$

Here $\mathrm{Col}(u)=\lambda(\mathcal L(f_u))$. The last map is surjective, since $m_1(\delta_1)=1$, and it has the cyclotomic action on its target. Its composition with $\mathrm{Col}$ is zero: $D\phi=p\phi D$ implies $D\mathcal L(f)(0)=0$. The kernel on the unit side consists of norm-compatible $p$-power [roots of unity](../../../algebra.md#root-of-unity). To see the shape of the kernel, write $z=\log(1+T)$; the equation $\mathcal L(f)=0$ becomes $h(pz)=ph(z)$ for $h(z)=\log f(e^z-1)$, so only its linear term can survive. Integral solutions are $f=(1+T)^c$, $c\in\mathbb Z_p$, after excluding finite residue factors by the [principal unit](../../../arithmetic.md#principal-unit) condition. For the image, use the following explicit [integral lifting of the corrected cyclotomic logarithm](../../../algebraic-number-theory.md#integral-lifting-of-the-corrected-cyclotomic-logarithm).

Take a [p-adic measure](../../../measure-theory.md#p-adic-measure) $\mu$ on the units with first moment zero, and write $g$ for its [Amice transform](../../../measure-theory.md#amice-transform). Then $Sg=0$ and $g'(0)=0$. Put $H=\exp(pg)\in1+pR$ and solve $f^p=H\phi(f)$ with $f(0)\in1+p\mathbb Z_p$. The constant equation is solved by $f_0=\exp(pg_0/(p-1))$. In degree one the terms involving $f_1$ cancel, and the remaining condition is $H_1=0$, exactly $g_1=0$; choose any $f_1\in\mathbb Z_p$. For $n\geq2$, after fixing the lower coefficients, the coefficient multiplying the unknown $f_n$ is

$$
p f_0^{p-1}(1-p^{n-1}).
$$

The other terms are divisible by $p$: for the already integral truncated series, $f^p\equiv\phi(f)\pmod p$, while $H\equiv1\pmod p$. Division therefore gives an integral $f_n$, since $f_0$ and $1-p^{n-1}$ are [units](../../../algebra.md#unit-in-a-ring). Recursion constructs $f\in R^\times$ with $\mathcal L(f)=g$. Now $pSg=\log(Nf/f)=0$, and $Nf/f\in1+pR$ by Question 2. The [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) is injective there, so $Nf=f$. This supplies the desired [Coleman power series](../../../algebraic-number-theory.md#coleman-power-series) of a [norm-compatible sequence of local units](../../../algebraic-number-theory.md#norm-compatible-sequence-of-local-units). The freely chosen linear coefficient accounts precisely for the kernel $(1+T)^c$. It proves the integral [surjectivity](../../../algebra.md#surjective-function) step, including the integrality that rational inversion of $1-\phi/p$ would leave unproved.

[Complex conjugation](../../../complex-analysis.md#complex-conjugation) acts by $-1$ on both copies of $\mathbb Z_p(1)$. As $p$ is odd, taking the even part is exact and removes both end terms. It follows that **$\mathrm{Col}:U_\infty^1\simeq\Lambda_G$**. The integral [exact sequence](../../../homology.md#exact-sequence) is essential here: the support calculation alone would not prove this [isomorphism](../../../algebra.md#isomorphism).

It remains to calculate the image of the [cyclotomic units](../../../galois-theory.md#cyclotomic-unit). For $a,b\in\mathbb Z_p^\times$, consider the [symmetric cyclotomic unit](../../../galois-theory.md#symmetric-cyclotomic-unit) series

$$
f_{a,b}(T)=X^{(b-a)/2}\frac{1-X^a}{1-X^b}.
$$

The quotient has an invertible constant term $a/b$, because both numerator and denominator have a simple zero at $T=0$. The factor $X^{(b-a)/2}$ makes the expression unchanged under $X\mapsto X^{-1}$. The product over the [roots of unity](../../../algebra.md#root-of-unity) gives $Nf_{a,b}=f_{a,b}$; one may verify this first for integer $a,b$ prime to $p$ and then extend by continuity. Dividing by the norm-compatible [Teichmuller representative](../../../arithmetic.md#teichmuller-representative) makes the series correspond to [principal units](../../../arithmetic.md#principal-unit) and does not change its logarithm. The generating function for the [Bernoulli numbers](../../../number-theory.md#bernoulli-number), with $z=\log X$, gives

$$
\log f_{a,b}(e^z-1)=\log(a/b)+\sum_{\substack{k\geq2\\k\text{ even}}}\frac{(a^k-b^k)B_k}{k\,k!}z^k.
$$

The symmetric factor cancels the linear term. Applying $1-\phi/p$, and then the moment formula of Question 3, yields

$$
\int x^k\,d\mathrm{Col}(f_{a,b})=(1-p^{k-1})(a^k-b^k)\frac{B_k}{k}=\int x^k\,d\bigl(([b]-[a])\zeta_p\bigr)
$$

for even $k\geq2$. These moments determine an even [p-adic measure](../../../measure-theory.md#p-adic-measure) on the units: [polynomials](../../../polynomial.md) are dense by the [Mahler theorem](../../../arithmetic.md#mahler-s-theorem), even projection preserves density, and multiplication by $x^2$ is invertible on the units, so the positive even-degree [polynomials](../../../polynomial.md) are dense there as well. Thus

$$
\mathrm{Col}(f_{a,b})=([b]-[a])\zeta_p.
$$

The closed ideal generated by all differences $[b]-[a]$ is $I(G)$. The closed [subgroup](../../../group.md#subgroup) generated by the corresponding [cyclotomic units](../../../galois-theory.md#cyclotomic-unit), including its [Galois group](../../../galois-theory.md#galois-group) translates, therefore has image exactly $I(G)\zeta_p$. Taking the quotient of the [isomorphism](../../../algebra.md#isomorphism) $U_\infty^1\simeq\Lambda_G$ proves the boxed local theorem.

Finally introduce global arithmetic. Let $\overline E_\infty^1$ be the closure of norm-compatible [global units](../../../algebraic-number-theory.md#global-unit-of-a-number-field) in the real tower, let $X_\infty^+$ be its [p-ramified Iwasawa module](../../../algebraic-number-theory.md#p-ramified-iwasawa-module), and let $Y_\infty^+$ be its [unramified Iwasawa module](../../../algebraic-number-theory.md#unramified-iwasawa-module). With compatible unit and splitting conventions, [class field theory](../../../algebraic-number-theory.md#class-field-theory) gives the [class-field unit sequence](../../../algebraic-number-theory.md#class-field-unit-sequence); quotienting its unit terms by $C_\infty^1$ gives

$$
0\longrightarrow\overline E_\infty^1/C_\infty^1\longrightarrow U_\infty^1/C_\infty^1\longrightarrow X_\infty^+\longrightarrow Y_\infty^+\longrightarrow0.
$$

In the cyclotomic tower the prime above $p$ is principal, so the unramified class-field convention also makes it split. On the torsion character components, multiplicativity of [characteristic ideals](../../../algebraic-number-theory.md#characteristic-ideal) implies

$$
\operatorname{char}(U_\infty^1/C_\infty^1)\operatorname{char}(Y_\infty^+)=\operatorname{char}(\overline E_\infty^1/C_\infty^1)\operatorname{char}(X_\infty^+).
$$

The local theorem has already calculated the first factor analytically. Equality of the [global unit](../../../algebraic-number-theory.md#global-unit-of-a-number-field) and class-group factors would therefore identify the [characteristic ideal](../../../algebraic-number-theory.md#characteristic-ideal) of $X_\infty^+$ with the same ideal of the [p-adic L-function](../../../analytic-number-theory.md#p-adic-l-function). That is the content predicted by the [Iwasawa main conjecture](../../../algebraic-number-theory.md#main-conjecture-of-iwasawa-theory). More explicitly, for a nontrivial even finite character $\chi$, the character component of $I(G)$ is the whole component and the prediction is

$$
\boxed{\operatorname{char}_{\Lambda_\chi}(X_\chi^+)=(g_\chi),\qquad g_\chi((1+p)^{1-s}-1)=L_p(\chi,s).}
$$

Here $\Lambda_\chi$ is the power-series algebra of the pro-$p$ part with coefficients in the character-value [ring](../../../commutative-algebra.md#ring). The trivial component requires the augmentation correction for the zeta pole. Equivalently the [characteristic ideals](../../../algebraic-number-theory.md#characteristic-ideal) of $\overline E_\infty^1/C_\infty^1$ and $Y_\infty^+$ agree componentwise. A formulation using odd class-group characters must include the appropriate cyclotomic twist and inversion, as in [Kummer reflection in Iwasawa theory](../../../galois-theory.md#kummer-reflection-in-iwasawa-theory). **The motivation is an analytic formula for [local units](../../../algebra.md#local-unit-of-a-local-field) together with a global class-field exact sequence; the global equality is the additional arithmetic assertion.**

The related class-number growth theorem illustrates why passage to an [Iwasawa module](../../../algebraic-number-theory.md#iwasawa-module) is powerful. For the cyclotomic $\mathbb Z_p$-extension, let $p^{e_n}$ be the $p$-part of the [class number](../../../algebraic-number-theory.md#class-number) at level $n$. The [unramified Iwasawa torsion theorem](../../../algebraic-number-theory.md#unramified-iwasawa-torsion-theorem), the [Iwasawa module structure theorem](../../../algebraic-number-theory.md#iwasawa-module-structure-theorem) and the class-group control relations give, for sufficiently large $n$,

$$
e_n=\mu p^n+\lambda n+\nu.
$$

Here $\mu,\lambda$ are the [Iwasawa invariants](../../../algebraic-number-theory.md#iwasawa-invariants). To see the two growth terms, use a topological generator $\gamma$ and, after a fixed sufficiently high level $n_0$, the norm polynomial $\nu_{n,n_0}=(\gamma^{p^n}-1)/(\gamma^{p^{n_0}}-1)$. An elementary summand $\Lambda/(p^a)$ contributes $a(p^n-p^{n_0})$ to the length of its quotient by this polynomial. A summand associated with a [distinguished polynomial](../../../arithmetic.md#distinguished-polynomial) of degree $d$ contributes $dn$ plus a constant: at each root $\alpha$ the valuation of the norm polynomial is $n$ plus a fixed constant for large $n$. If $1+\alpha$ is a root of unity already killed at level $n_0$, its value is instead exactly $p^{n-n_0}$ and gives the same linear contribution. The finite errors in the structure and control maps stabilize and contribute to $\nu$. Thus module structure explains growth, while the [Iwasawa main conjecture](../../../algebraic-number-theory.md#main-conjecture-of-iwasawa-theory) goes further by identifying the [characteristic series of an Iwasawa module](../../../algebraic-number-theory.md#characteristic-series-of-an-iwasawa-module) themselves with analytic ones.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
