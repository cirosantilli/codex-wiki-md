# Paper 26

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper26.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper26.pdf)

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
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $q=e^{2\pi i\tau}$ and $\sigma_j(n)=\sum_{d\mid n}d^j$. Separate the $m=0$ terms in the [lattice Eisenstein series](../../../modular-function.md#lattice-eisenstein-sum). Differentiating the [cosecant partial-fraction identity](../../../fourier-series.md#cosecant-partial-fraction-identity) $2k-2$ times gives, for $\Im z>0$,

$$
\sum_{n\in\mathbb Z}(z+n)^{-2k}
=\frac{(2\pi i)^{2k}}{(2k-1)!}\sum_{r\geq1}r^{2k-1}e^{2\pi irz}.
$$

The initial identity is $\sum_n(z+n)^{-2}=\pi^2\csc^2(\pi z)=-4\pi^2\sum_{r\geq1}re^{2\pi irz}$; differentiation accounts for the factorial and the sign. Pair $m$ and $-m$ and collect the products $mr$. [Absolute convergence](../../../real-analysis.md#absolute-convergence) of the lattice sum for $k\geq2$, and local uniform convergence of the resulting [power series](../../../real-analysis.md#power-series), justify these operations. Thus the requested [Fourier expansions](../../../fourier-series.md) are

$$
\boxed{G_{2k}(\tau)=2\zeta(2k)+\frac{2(2\pi i)^{2k}}{(2k-1)!}\sum_{n\geq1}\sigma_{2k-1}(n)q^n,\qquad
E_{2k}(\tau)=1-\frac{4k}{B_{2k}}\sum_{n\geq1}\sigma_{2k-1}(n)q^n.}
$$

Here $E_{2k}=G_{2k}/(2\zeta(2k))$, and the [Bernoulli numbers](../../../number-theory.md#bernoulli-number) have convention $B_2=1/6$. The second formula uses Euler's even-value identity for the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function), $2\zeta(2k)=(-1)^{k+1}B_{2k}(2\pi)^{2k}/(2k)!$. In particular $E_4=1+240\sum\sigma_3(n)q^n$ and $E_6=1-504\sum\sigma_5(n)q^n$.

We need the rational, rather than merely complex, version of the [polynomial ring of level-one modular forms](../../../modular-function.md#polynomial-ring-of-level-one-modular-forms). Recall how the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group) supplies its proof. For a nonzero weight-$w$ [modular form](../../../modular-function.md#modular-form), with $\rho=e^{2\pi i/3}$,

$$
v_\infty(f)+\tfrac12v_i(f)+\tfrac13v_\rho(f)+\sum_{z\ne i,\rho}v_z(f)=w/12.
$$

Integrate $f'/f$ around a truncated [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group), indenting around boundary zeros. The paired vertical sides cancel by translation; pair the two halves of the circular edge using $f(-1/\tau)=\tau^wf(\tau)$. The logarithmic derivative of $\tau^w$ supplies $w/12$, while the top edge supplies $v_\infty(f)$. The half-disc and third-disc at the two elliptic points account for the fractions $1/2,1/3$. The [argument principle](../../../complex-analysis.md#argument-principle) then gives the formula. All orders in it are nonnegative for a holomorphic [modular form](../../../modular-function.md#modular-form). It follows that negative weights have no forms, $M_0=\mathbb C$, and $M_2=0$: a weight-two form vanishes at $i$, contributing at least $1/2>2/12$.

Define $\Delta_0=(E_4^3-E_6^2)/1728$. It is a weight-twelve [cusp form](../../../modular-function.md#cusp-form) and its expansion starts with $q$. The [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group) forces its order at infinity to be exactly one and leaves no interior zeros. Thus division by $\Delta_0$ identifies $S_w$ with $M_{w-12}$. Every nonnegative even $w\ne2$ has a monomial $E_4^aE_6^b$ of weight $w$: solve $2a+3b=w/2$, taking $b=0$ when $w/2$ is even and $b=1$ when it is odd and at least three. Subtract the constant coefficient of a [modular form](../../../modular-function.md#modular-form) times such a monomial and divide by $\Delta_0$. Induction on weight proves generation by $E_4,E_6$.

If the original [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are rational, every step preserves rationality: both generators and $\Delta_0$ have rational expansions, and formal division by $\Delta_0=q+O(q^2)$ does too. This proves the [rational structure of level-one modular forms](../../../modular-function.md#rational-structure-of-level-one-modular-forms). Write $E_{2k}=\sum r_{a,b}E_4^aE_6^b$ with $r_{a,b}\in\mathbb Q$ and $4a+6b=2k$. Rescaling gives

$$
G_{2k}=\sum_{4a+6b=2k}r_{a,b}\frac{2\zeta(2k)}{(2\zeta(4))^a(2\zeta(6))^b}G_4^aG_6^b.
$$

The [Bernoulli number](../../../number-theory.md#bernoulli-number) formula above makes each zeta ratio rational: its powers of $\pi$ cancel precisely because the weights agree. This proves the required rational coefficients for the unnormalized [lattice Eisenstein sums](../../../modular-function.md#lattice-eisenstein-sum).

Finally $S_8=S_{10}=0$ because the quotient weights are negative, and $S_{14}=0$ because $M_2=0$. In each of these weights a form is determined by its constant coefficient. The indicated monomials have that coefficient equal to one, so

$$
\boxed{E_8=E_4^2,\qquad E_{10}=E_4E_6,\qquad E_{14}=E_4^2E_6.}
$$

## 2

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb Z)$ and $j=c\tau+d$. Differentiating the transformation law of a weight-$k$ [modular form](../../../modular-function.md#modular-form) gives the [derivative transformation of a weak modular form](../../../modular-function.md#derivative-transformation-of-a-weak-modular-form)

$$
(Df)(\gamma\tau)=j^{k+2}Df(\tau)+\frac{kc}{2\pi i}j^{k+1}f(\tau).
$$

The corresponding anomaly for $Dg$ has coefficient $\ell c/(2\pi i)$. Consequently these anomalies cancel in $\ell gDf-kfDg$, which transforms with weight $k+\ell+2$. The [derivatives](../../../calculus.md#derivative) are holomorphic on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). In a [Fourier expansion](../../../fourier-series.md), $D(\sum_{n\geq0}a_nq^n)=\sum_{n\geq1}na_nq^n$, so each term in the combination has zero constant coefficient and no negative powers. There is just one [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) up to the full [modular group](../../../modular-function.md#modular-group). Therefore

$$
\boxed{\ell gDf-kfDg\in S_{k+\ell+2}.}
$$

This is, up to the chosen sign, the [first Rankin-Cohen bracket](../../../modular-function.md#first-rankin-cohen-bracket).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The required anomaly cancellation depends on the exact [Eisenstein series of weight two](../../../modular-function.md#eisenstein-series-of-weight-two) law

$$
E_2(\gamma\tau)=j^2E_2(\tau)+\frac{12c}{2\pi i}j,\qquad j=c\tau+d.
$$

Here is a way to establish it without assuming that $E_2$ is a [modular form](../../../modular-function.md#modular-form). The lattice definition of the [completed nonholomorphic Eisenstein series](../../../modular-function.md#completed-nonholomorphic-eisenstein-series) in Question 6 is [modular invariant](../../../modular-function.md#modular-invariant-function). Its [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) calculation, proved there, gives the finite Laurent coefficient at $s=1$ as

$$
C(\tau)=\frac{\gamma_E-\log(4\pi)}2-\frac12\log y+\frac{\pi y}{6}-2\sum_{n\geq1}\log|1-q^n|,\qquad y=\Im\tau.
$$

The residue is constant, so $C$ is also invariant. This calculation uses only convergent Gaussian integrals and the analytic infinite product, not modularity of that product. Using the [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives) $\partial_\tau$, with $\partial_\tau y=1/(2i)$, differentiation of the locally uniformly convergent series gives

$$
\partial_\tau C=-\frac{\pi i}{12}\left(E_2(\tau)-\frac3{\pi y}\right).
$$

Differentiate $C(\gamma\tau)=C(\tau)$ to see that $E_2^*=E_2-3/(\pi y)$ transforms with weight two. Substituting $\Im(\gamma\tau)=y/|j|^2$ yields

$$
E_2(\gamma\tau)-j^2E_2(\tau)=\frac3{\pi y}(|j|^2-j^2)
=\frac{12c}{2\pi i}j,
$$

since $\overline j-j=-2icy$. This is the [weight-two transformation from an invariant Eisenstein limit](../../../modular-function.md#weight-two-transformation-from-an-invariant-eisenstein-limit).

Combine this law with the [derivative transformation of a weak modular form](../../../modular-function.md#derivative-transformation-of-a-weak-modular-form) proved in part (i). The anomalous terms in $Df-(k/12)E_2f$ cancel exactly, leaving the weight-$k+2$ transformation law. Both functions are holomorphic on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), and their [Fourier expansions](../../../fourier-series.md) contain no negative powers. Hence the [Serre derivative](../../../modular-function.md#serre-derivative) satisfies

$$
\boxed{D_kf:=Df-\frac{k}{12}E_2f\in M_{k+2}.}
$$

Its constant coefficient is $-ka_0(f)/12$; it need not be a [cusp form](../../../modular-function.md#cusp-form) when $f$ is not cuspidal.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The product defining the [modular discriminant](../../../modular-function.md#modular-discriminant) converges locally uniformly for $|q|<1$ and has integral [Fourier coefficients](../../../fourier-series.md#fourier-coefficient). Its [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) is

$$
D\log\left(q\prod_{r\geq1}(1-q^r)^{24}\right)
=1-24\sum_{r\geq1}\frac{rq^r}{1-q^r}
=1-24\sum_{n\geq1}\sigma_1(n)q^n=E_2.
$$

Therefore $D\Delta=E_2\Delta$. Comparing the coefficient of $q^n$ gives $n\tau(n)=\tau(n)-24\sum_{j=1}^{n-1}\sigma_1(j)\tau(n-j)$, or

$$
\boxed{(1-n)\tau(n)=24\sum_{j=1}^{n-1}\sigma_1(j)\tau(n-j).}
$$

This also fixes the initial value $\tau(1)=1$.

For the [Ramanujan tau congruence modulo five](../../../modular-function.md#ramanujan-tau-congruence-modulo-five), first justify the link between this product and $E_4,E_6$. Question 1 constructs $\Delta_0=(E_4^3-E_6^2)/1728\in S_{12}$ with first coefficient one. Its [Serre derivative](../../../modular-function.md#serre-derivative) is in $S_{14}$, which vanishes by the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group): a nonzero such [cusp form](../../../modular-function.md#cusp-form) would contribute at least $1+1/2>14/12$, since it vanishes at infinity and at $i$. Hence $D\Delta_0=E_2\Delta_0$. The product and $\Delta_0$ have the same [differential equation](../../../differential-equation.md) and leading coefficient. Equivalently their quotient has derivative zero near $q=0$ and limit one; the [identity theorem](../../../complex-analysis.md#identity-theorem) gives

$$
1728\Delta=E_4^3-E_6^2.
$$

Also $D_6E_6\in M_8=\mathbb C E_4^2$. Its constant coefficient is $-1/2$, so the [Serre derivative](../../../modular-function.md#serre-derivative) gives $2DE_6=E_2E_6-E_4^2$.

Work now in the [formal power series](../../../commutative-algebra.md#formal-power-series) ring $\mathbb F_5[[q]]$. The integral expansions give $E_4\equiv1$ and $E_2\equiv E_6\pmod5$, because $d^5\equiv d\pmod5$, $-24\equiv-504\equiv1$, and $240\equiv0$. The two identities reduce to

$$
3\Delta\equiv1-E_6^2,\qquad 2DE_6\equiv E_6^2-1\pmod5.
$$

Thus $3\Delta\equiv-2DE_6\equiv3DE_6$, and division by the nonzero element $3$ gives $\Delta\equiv DE_6$. Since the coefficient of $q^n$ in $DE_6$ is $-504n\sigma_5(n)$, we conclude

$$
\boxed{\tau(n)\equiv n\sigma_5(n)\pmod5\quad(n\geq1).}
$$

## 3

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Extend $\chi$ by zero to integers not coprime to $N$, and write $g(\chi)=\sum_{a\bmod N}\chi(a)e^{2\pi ia/N}$ for its [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character). We use the analytic branch of $\sqrt{-i\tau}$ that is positive when $\tau$ is positive imaginary. With the convention $\widehat F(t)=\int_{\mathbb R}F(x)e^{-2\pi ixt}\,dx$, the [Gaussian Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-gaussian) and its differentiated version are

$$
\widehat{e^{\pi i\tau x^2}}(t)=(-i\tau)^{-1/2}e^{-\pi it^2/\tau},\qquad
\widehat{x e^{\pi i\tau x^2}}(t)=\frac{t}{\tau}(-i\tau)^{-1/2}e^{-\pi it^2/\tau}.
$$

The first formula follows by completing the square, first on the imaginary axis and then by [analytic continuation](../../../complex-analysis.md#analytic-continuation); the second follows by differentiating the [Fourier transform](../../../analysis.md#fourier-transform) in $t$. All the functions are [Schwartz functions](../../../fourier-analysis.md#schwartz-function) on the real axis.

For completeness, the [finite Fourier transform of a primitive Dirichlet character](../../../algebraic-number-theory.md#finite-fourier-transform-of-a-primitive-dirichlet-character) satisfies

$$
\sum_{a\bmod N}\chi(a)e^{2\pi ira/N}=g(\chi)\overline\chi(r).
$$

For a unit $r$ this is substitution by its inverse. If $p\mid(r,N)$, primitivity supplies a unit $u\equiv1\pmod{N/p}$ with $\chi(u)\ne1$: otherwise the character would factor through modulus $N/p$. Multiplication by $u$ fixes the additive exponential but multiplies the sum by $\chi(u)$, so the sum vanishes. This proves the identity also on nonunits. Finite [Parseval identity](../../../fourier-analysis.md#parseval-identity) now gives $|g(\chi)|^2=N$, since exactly $\varphi(N)$ frequencies have nonzero character values. In particular this [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) is nonzero.

Apply [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) to each residue class: $\sum_jF(a+Nj)=N^{-1}\sum_r e^{2\pi ira/N}\widehat F(r/N)$. Multiply by $\chi(a)$ and sum over $a$. The formulas above give the two [character theta transformations](../../../algebraic-number-theory.md#character-theta-transformation)

$$
\boxed{\theta_\chi(\tau)=\frac{g(\chi)}{N\sqrt{-i\tau}}\,
\theta_{\overline\chi}\!\left(-\frac1{N^2\tau}\right)\quad\text{if }\chi(-1)=1,}
$$

and

$$
\boxed{\widetilde\theta_\chi(\tau)=\frac{g(\chi)}{iN^2(-i\tau)^{3/2}}\,
\widetilde\theta_{\overline\chi}\!\left(-\frac1{N^2\tau}\right)\quad\text{if }\chi(-1)=-1.}
$$

In the odd case the prefactor originally reads $g(\chi)/(N^2\tau\sqrt{-i\tau})$; using $\tau=i(-i\tau)$ explains the factor $i$. Opposite parity makes the corresponding series identically zero by pairing $n,-n$. This is why the weight-three-halves series is needed for odd [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character).

To deduce the products from these transformations, use two specific [primitive Dirichlet characters](../../../algebraic-number-theory.md#primitive-dirichlet-character). The even character $\chi_{12}$ takes values $1,-1,-1,1$ on $1,5,7,11$ modulo twelve. It is primitive: its values do not factor through six or four, hence through no proper divisor of twelve. Its [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) is $2\sqrt3=\sqrt{12}$. Put

$$
A(\tau)=\tfrac12\theta_{\chi_{12}}(\tau/12)=\tfrac12\sum_n\chi_{12}(n)q^{n^2/24}.
$$

The even transformation gives $A(-1/\tau)=\sqrt{-i\tau}\,A(\tau)$; also $A(\tau+1)=e^{\pi i/12}A(\tau)$, since each nonzero term has $n^2\equiv1\pmod{24}$. Thus $A^{24}$ transforms as a weight-twelve [modular form](../../../modular-function.md#modular-form) under the generators $S,T$ of the [modular group](../../../modular-function.md#modular-group). It is holomorphic and starts with $q$, so it is a normalized [cusp form](../../../modular-function.md#cusp-form). The proof in Question 1 shows $S_{12}=\mathbb C\Delta_0$, giving $A^{24}=\Delta_0$. In particular $A$ has no interior zeros, by the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group).

The [Serre derivative](../../../modular-function.md#serre-derivative) argument in Question 2 gives $D\Delta_0=E_2\Delta_0$. Hence $DA/A=E_2/24$. The analytic product $P(\tau)=q^{1/24}\prod_{n\geq1}(1-q^n)$ is nonzero and has the same [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative), since $DP/P=1/24-\sum\sigma_1(n)q^n$. Therefore $A/P$ is constant on the connected [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis); its limit at infinity is one. This proves $A=P$, without assuming either of the product identities being deduced. Pair the terms $n,-n$ in $A$, choosing representatives $n=6r+1$. Since $\chi_{12}(6r+1)=(-1)^r$, we get

$$
A=q^{1/24}\sum_{r\in\mathbb Z}(-1)^r q^{r(3r+1)/2},
\qquad
\boxed{\prod_{n\geq1}(1-q^n)=\sum_{r\in\mathbb Z}(-1)^r q^{r(3r+1)/2}.}
$$

This is the [Euler pentagonal identity](../../../modular-function.md#euler-pentagonal-identity), derived by the [character theta proof of the eta product](../../../algebraic-number-theory.md#character-theta-proof-of-the-eta-product).

For the second product use the odd primitive character $\chi_4(1)=1$, $\chi_4(3)=-1$, with [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) $2i$. Set

$$
B(\tau)=\tfrac12\widetilde\theta_{\chi_4}(\tau/4)=\tfrac12\sum_n n\chi_4(n)q^{n^2/8}.
$$

The odd transformation gives $B(-1/\tau)=(-i\tau)^{3/2}B(\tau)$ and the series gives $B(\tau+1)=e^{\pi i/4}B(\tau)$. Thus $B^8$ is another normalized weight-twelve [cusp form](../../../modular-function.md#cusp-form), and $B^8=\Delta_0=A^{24}$. Because $A$ is nonzero, $B/A^3$ has eighth power one, so it is constant; its leading coefficient fixes it to one. Pairing positive and negative odd integers now gives

$$
B=q^{1/8}\sum_{r\geq0}(-1)^r(2r+1)q^{r(r+1)/2}.
$$

Since $B=A^3=q^{1/8}\prod_{n\geq1}(1-q^n)^3$, the [Jacobi cubic product identity](../../../modular-function.md#jacobi-cubic-product-identity) follows:

$$
\boxed{\prod_{n\geq1}(1-q^n)^3=\sum_{r\geq0}(-1)^r(2r+1)q^{r(r+1)/2}.}
$$

All pairings and differentiations take place in locally uniformly convergent [theta functions](../../../modular-function.md#theta-function) or products on $|q|<1$.

## 4

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $\Gamma=SL_2(\mathbb Z)$ and use the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator)

$$
(f|_k\alpha)(\tau)=(\det\alpha)^{k/2}(c\tau+d)^{-k}f(\alpha\tau),\qquad
\alpha=\begin{pmatrix}a&b\\c&d\end{pmatrix},\quad\det\alpha>0.
$$

The [automorphy factor](../../../modular-function.md#automorphy-factor) identity proves $(f|_k\alpha)|_k\beta=f|_k(\alpha\beta)$, and positive scalar matrices act trivially. Let $\mathcal M_n$ be all integral matrices of determinant $n>0$. It is stable under left and right multiplication by $\Gamma$. Its left orbits have unique representatives

$$
\Pi_n=\left\{\begin{pmatrix}a&b\\0&d\end{pmatrix}:ad=n,\ a,d>0,\ 0\leq b<d\right\}.
$$

Indeed [Bézout's identity](../../../algebra.md#bezout-identity) reduces the first column to $(a,0)$, the determinant fixes $d=n/a$, and a row shear reduces $b$ modulo $d$. These are the [determinant-n matrix representatives for Hecke operators](../../../modular-function.md#determinant-n-matrix-representatives-for-hecke-operators). For composite $n$, $\mathcal M_n$ can contain more than one double coset; keeping every integral matrix, including nonprimitive ones, is essential.

Define the [Hecke operator](../../../modular-function.md#hecke-operator) by

$$
\boxed{T_nf=n^{k/2-1}\sum_{\alpha\in\Pi_n}f|_k\alpha
=n^{k-1}\sum_{ad=n}d^{-k}\sum_{b=0}^{d-1}f\left(\frac{a\tau+b}{d}\right).}
$$

Changing a representative on the left leaves its summand unchanged. Right multiplication by $\Gamma$ permutes left orbits of $\mathcal M_n$, so the result satisfies the weight-$k$ transformation law. Each summand is holomorphic. Its expansion at infinity is bounded, and vanishes there when $f$ is a [cusp form](../../../modular-function.md#cusp-form); the group has just one cusp class. Therefore $T_n$ preserves both $M_k$ and $S_k$, and $T_1$ is the identity.

For a [Fourier expansion](../../../fourier-series.md) $f=\sum_{r\geq0}a_rq^r$, the sum over $b$ vanishes unless $d\mid r$. Substitute $r=dt$ and then collect the coefficient of $q^m$ to obtain the [Fourier coefficients of a composite-index Hecke operator](../../../modular-function.md#fourier-coefficients-of-a-composite-index-hecke-operator):

$$
\boxed{a_m(T_nf)=\sum_{h\mid\gcd(m,n)}h^{k-1}a_{mn/h^2}(f).}
$$

Here $\gcd(0,n)=n$, so the constant coefficient is $\sigma_{k-1}(n)a_0$; at $m=1$ it is $a_n$. This proves preservation of integral coefficients. At a prime,

$$
T_pf=p^{k-1}f(p\tau)+\frac1p\sum_{b=0}^{p-1}f((\tau+b)/p),\qquad
 a_m(T_pf)=a_{pm}+p^{k-1}a_{m/p},
$$

with $a_{m/p}=0$ if $p\nmid m$.

We can prove the entire [Hecke multiplication relations](../../../modular-function.md#hecke-multiplication-relations) directly, not just quote them. On [formal power series](../../../commutative-algebra.md#formal-power-series) put $U_p(\sum a_mq^m)=\sum a_{pm}q^m$ and $V_p f(q)=f(q^p)$. Although these individual operators need not preserve level one, $U_pV_p=1$ and the coefficient formula gives

$$
T_{p^r}=\sum_{j=0}^r p^{j(k-1)}V_p^jU_p^{r-j}.
$$

Multiply on the left by $T_p=U_p+p^{k-1}V_p$. In the first part the $j=0$ term is $U_p^{r+1}$; every $j\geq1$ reduces by $U_pV_p=1$ to $p^{j(k-1)}V_p^{j-1}U_p^{r-j}$. The second part, together with the $j=0$ term, is $T_{p^{r+1}}$. The remaining sum is $p^{k-1}T_{p^{r-1}}$. Thus

$$
T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}\quad(r\geq1).
$$

For coprime indices, the coefficient divisors split independently in the displayed formula, proving $T_mT_n=T_{mn}$ when $(m,n)=1$. Induction with the prime-power recurrence gives $T_{p^r}T_{p^t}=\sum_{j=0}^{\min(r,t)}p^{j(k-1)}T_{p^{r+t-2j}}$. Combining the primes proves

$$
\boxed{T_mT_n=\sum_{h\mid\gcd(m,n)}h^{k-1}T_{mn/h^2}.}
$$

In particular the [modular Hecke algebra](../../../modular-function.md#modular-hecke-algebra) is commutative and is generated by the prime operators.

For [cusp forms](../../../modular-function.md#cusp-form) the [Petersson inner product](../../../modular-function.md#petersson-inner-product) is

$$
\langle f,g\rangle=\int_{\Gamma\backslash\mathbb H}f(\tau)\overline{g(\tau)}y^k\frac{dx\,dy}{y^2}.
$$

Cusp decay makes it finite and positive definite. The [Hecke operators are self-adjoint for the Petersson inner product](../../../modular-function.md#hecke-operators-are-self-adjoint-for-the-petersson-inner-product). To see the change-of-variables mechanism, fix a double coset $\Gamma\alpha\Gamma\subset\mathcal M_n$ and put $H=\Gamma\cap\alpha^{-1}\Gamma\alpha$. Representatives $\gamma$ of $H\backslash\Gamma$ give left representatives $\alpha\gamma$. Unfolding the sum in $\langle\sum_\gamma f|_k\alpha\gamma,g\rangle$ changes the integral over $\Gamma\backslash\mathbb H$ to the integral over $H\backslash\mathbb H$ of $(f|_k\alpha)\overline g$. The substitution $w=\alpha\tau$ preserves $dx\,dy/y^2$ and has $\Im w=(\det\alpha)y/|c\tau+d|^2$; these factors move the slash from $f$ to $g|_k\alpha^{-1}$. Refold over $\alpha H\alpha^{-1}=\Gamma\cap\alpha\Gamma\alpha^{-1}$ to get the reverse double coset. Since scalar matrices act trivially, $\alpha^{-1}$ has the same slash action as its adjugate $\alpha^*=n\alpha^{-1}$, an integral matrix of determinant $n$. The adjugate involution permutes all the double cosets in $\mathcal M_n$. The common real factor $n^{k/2-1}$ is unchanged, giving $\langle T_nf,g\rangle=\langle f,T_ng\rangle$.

Since $S_k$ is finite dimensional, commuting self-adjoint [linear operators](../../../vector-space.md#linear-operator) have a common [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [Hecke eigenforms](../../../modular-function.md#hecke-eigenform): diagonalize one operator, restrict the others to its eigenspaces, and repeat until these spaces cannot split further. If $f$ is a nonzero common [Hecke eigenform](../../../modular-function.md#hecke-eigenform) with $T_nf=\lambda_nf$, the coefficient at $q$ gives $a_n=\lambda_na_1$. Were $a_1=0$, every positive coefficient would vanish, contrary to $f\ne0$ being cuspidal. Normalize $a_1=1$; then $\lambda_n=a_n$, and the [Hecke multiplication relations](../../../modular-function.md#hecke-multiplication-relations) yield

$$
a_ma_n=\sum_{h\mid\gcd(m,n)}h^{k-1}a_{mn/h^2},\qquad
a_{p^{r+1}}=a_pa_{p^r}-p^{k-1}a_{p^{r-1}}.
$$

The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real by self-adjointness. Their multiplicativity and prime-power recurrence give the [Euler product of a Hecke eigenform](../../../modular-function.md#euler-product-of-a-hecke-eigenform), initially in an absolutely convergent half-plane:

$$
\boxed{L(f,s)=\prod_p\left(1-a_pp^{-s}+p^{k-1-2s}\right)^{-1}.}
$$

The [Mellin transform](../../../analysis.md#mellin-transform) in Question 5 supplies its analytic continuation and functional equation.

Finally, for positive even $k\geq4$, $M_k=\mathbb C E_k\oplus S_k$, by subtracting the constant coefficient times the normalized [Eisenstein series](../../../modular-function.md#eisenstein-series). The divisor identity

$$
\sigma_{k-1}(m)\sigma_{k-1}(n)=\sum_{h\mid\gcd(m,n)}h^{k-1}\sigma_{k-1}(mn/h^2)
$$

follows by multiplying the geometric sums at each prime; it and the constant-coefficient formula prove $T_nE_k=\sigma_{k-1}(n)E_k$. Thus $M_k$ has an [Eisenstein series](../../../modular-function.md#eisenstein-series) eigenline and a basis of cuspidal [Hecke eigenforms](../../../modular-function.md#hecke-eigenform). Odd and negative weights have no forms, $M_2=0$, and on $M_0=\mathbb C$ the operator is the scalar $\sigma_{-1}(n)$. These statements fix the normalization and describe the exceptional small weights as well.

## 5

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $a_0$ be the constant [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) and suppose first that $k>0$ is even and $M_k\ne0$; thus $k\geq4$. Put $\varepsilon=i^k=(-1)^{k/2}$. The precise [Mellin continuation of a noncuspidal modular form](../../../modular-function.md#mellin-continuation-of-a-noncuspidal-modular-form) is

$$
\boxed{\Lambda_f(s)=(2\pi)^{-s}\Gamma(s)L(f,s),\qquad
\Lambda_f(s)=\varepsilon\Lambda_f(k-s).}
$$

It is [meromorphic](../../../isolated-singularity.md#meromorphic-function) on the whole plane, with possible simple [poles](../../../isolated-singularity.md#pole) only at $0,k$, of residues $-a_0,\varepsilon a_0$, respectively. For a [cusp form](../../../modular-function.md#cusp-form) it is an [entire function](../../../complex-analysis.md#entire-function). A nonzero constant term makes both of these poles genuine.

We first justify the initial [Mellin transform](../../../analysis.md#mellin-transform). Decompose $f=a_0E_k+h$ with $h\in S_k$. For a [cusp form](../../../modular-function.md#cusp-form), $y^{k/2}|h(x+iy)|$ is invariant under the [modular group](../../../modular-function.md#modular-group) and bounded on its fundamental domain, since it tends to zero at the cusp. Therefore it is bounded throughout the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Integrating the [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) at height $y=1/n$ gives $|a_n(h)|\leq Ce^{2\pi}n^{k/2}$. The [Eisenstein series](../../../modular-function.md#eisenstein-series) coefficients satisfy $\sigma_{k-1}(n)\leq\zeta(k-1)n^{k-1}$ by replacing divisors $d$ by $n/d$. Consequently $a_n(f)=O(n^{k-1})$, and absolute termwise integration is valid for $\Re s>k$:

$$
\Lambda_f(s)=\int_0^\infty(f(iy)-a_0)y^{s-1}\,dy.
$$

Indeed $\int_0^\infty e^{-2\pi ny}y^{s-1}\,dy=(2\pi n)^{-s}\Gamma(s)$, and the sum of the absolute integrals converges in that half-plane.

Write $I_f(s)=\int_1^\infty(f(iy)-a_0)y^{s-1}\,dy$. Exponential cusp decay of the difference implies uniform convergence on compact subsets of the $s$-plane, including after any number of derivatives in $s$, so $I_f$ is entire. The modular transformation $f(i/y)=(iy)^kf(iy)$ gives

$$
f(iy)=\varepsilon y^{-k}f(i/y).
$$

On the lower half of the Mellin integral, subtract the transformed constant explicitly:

$$
f(iy)-a_0=\varepsilon y^{-k}(f(i/y)-a_0)+a_0(\varepsilon y^{-k}-1).
$$

Substitute $y=1/t$ in the decaying term and integrate the two powers in the constant term. This yields, initially for $\Re s>k$,

$$
\boxed{\Lambda_f(s)=I_f(s)+\varepsilon I_f(k-s)+a_0\left(\frac{\varepsilon}{s-k}-\frac1s\right).}
$$

The right side supplies the claimed [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) and its residues. Replacing $s$ by $k-s$ and multiplying by $\varepsilon$, with $\varepsilon^2=1$, leaves this expression unchanged, proving the [functional equation](../../../analysis.md#functional-equation) with its correct sign. In particular the residue at $k$ is tied to the residue at zero by that equation; subtracting only $a_0$ at infinity and overlooking its transformed value at zero would miss these poles.

In weight zero every [modular form](../../../modular-function.md#modular-form) is constant, so $L(f,s)=0$ and its completion is identically zero. The same holds for the zero form in odd, negative, or weight-two spaces. Thus the assertion covers all weights in the notation of the paper. There is no conjugation of $f$ in this level-one functional equation.

## 6

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use $\Xi(u)=\pi^{-u/2}\Gamma(u/2)\zeta(u)$ for the [completed Riemann zeta function](../../../analytic-number-theory.md#completed-riemann-zeta-function), without the polynomial factor used to define the entire [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function). For complex $\nu$ put

$$
K_\nu(Y)=\frac12\int_0^\infty e^{-Y(t+t^{-1})/2}t^{\nu-1}\,dt,\qquad Y>0.
$$

This is the [Modified Bessel function of the second kind](../../../analysis.md#modified-bessel-function-of-the-second-kind). The substitution $t=e^v$ writes it as $\tfrac12\int_{\mathbb R}e^{-Y\cosh v+\nu v}\,dv$, proving that it is entire in $\nu$, that $K_\nu=K_{-\nu}$, and that it decays exponentially as $Y\to\infty$, uniformly for $\nu$ in a compact set.

For $\Re s>1$ all the lattice sums and the integrals below converge absolutely. The $m=0$ terms in the [completed nonholomorphic Eisenstein series](../../../modular-function.md#completed-nonholomorphic-eisenstein-series) contribute $\Xi(2s)y^s$. For $m\ne0$, use the [Gamma integral](../../../complex-analysis.md#gamma-integral) and then [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) in $n$:

$$
\begin{aligned}
\mathcal E(z,s)-\Xi(2s)y^s
&=\frac{y^s}{2}\sum_{m\ne0}\int_0^\infty u^{s-1}e^{-\pi m^2y^2u}\sum_n e^{-\pi u(n+mx)^2}\,du\\
&=\frac{y^s}{2}\sum_{m\ne0}\sum_{h\in\mathbb Z}e^{2\pi ihmx}
\int_0^\infty u^{s-3/2}e^{-\pi m^2y^2u-\pi h^2/u}\,du.
\end{aligned}
$$

Here the Poisson identity is $\sum_n e^{-\pi u(n+mx)^2}=u^{-1/2}\sum_h e^{-\pi h^2/u}e^{2\pi ihmx}$. At $h=0$, evaluating the [Gamma integral](../../../complex-analysis.md#gamma-integral) and summing over $m$ gives $\Xi(2s-1)y^{1-s}$. At $h\ne0$, the substitution $u=|h|t/(|m|y)$ and the [integral representation of the modified Bessel function of the second kind](../../../analysis.md#integral-representation-of-the-modified-bessel-function-of-the-second-kind) give

$$
\int_0^\infty u^{s-3/2}e^{-\pi m^2y^2u-\pi h^2/u}\,du
=2\left(\frac{|h|}{|m|y}\right)^{s-1/2}K_{s-1/2}(2\pi|mh|y).
$$

Collect the frequency $r=mh\ne0$. There are two signed choices of $m$ for each positive divisor of $|r|$. Thus, with $\sigma_a(n)=\sum_{d\mid n}d^a$, the full [Fourier expansion](../../../fourier-series.md) is

$$
\boxed{\mathcal E(z,s)=\Xi(2s)y^s+\Xi(2s-1)y^{1-s}
+2\sqrt y\sum_{r\ne0}|r|^{s-1/2}\sigma_{1-2s}(|r|)K_{s-1/2}(2\pi|r|y)e^{2\pi irx}.}
$$

The factor $2$ is important: the lattice sum includes both signs, while the defining factor $1/2$ was already used in its Mellin integral. This expansion uses exactly the completion in the question.

We can deduce both of the offered conclusions. First recall, with a short proof, the needed [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function). Put $\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}$. [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) gives $\Theta(t)=t^{-1/2}\Theta(1/t)$. Splitting the Mellin integral of $\Theta-1$ at one yields

$$
\Xi(u)=-\frac1u-\frac1{1-u}
+\frac12\int_1^\infty(\Theta(t)-1)\left(t^{u/2-1}+t^{(1-u)/2-1}\right)\,dt.
$$

The integral is entire and invariant under $u\mapsto1-u$. Hence $\Xi(u)=\Xi(1-u)$, with only simple [poles](../../../isolated-singularity.md#pole) at $u=0,1$, of residues $-1,1$. This is the pole-bearing completion, not the entire xi function.

For fixed $y>0$, the nonconstant part of the Eisenstein expansion is entire in $s$ and locally normally convergent: the [divisor sums](../../../number-theory.md#divisor-sum) grow at most polynomially on a compact set of $s$, whereas $K_{s-1/2}(2\pi|r|y)$ decays exponentially in $|r|$. The same argument gives local uniformity for $z$ in compact subsets of the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Thus only the constant terms can have poles. Their apparent poles at $s=1/2$ cancel: $\Xi(2s)$ has principal part $1/(2(s-1/2))$, while $\Xi(2s-1)$ has its negative, and both multiply $y^{1/2}$ there. The remaining poles are simple, at $s=0,1$, with residues $-1/2,1/2$.

Under $s\mapsto1-s$, the two constant terms interchange by the zeta functional equation. The nonconstant terms are unchanged because $K_\nu=K_{-\nu}$ and

$$
|r|^{s-1/2}\sigma_{1-2s}(|r|)=|r|^{1/2-s}\sigma_{2s-1}(|r|),
$$

which follows by replacing a divisor $d$ by $|r|/d$. Therefore

$$
\boxed{\mathcal E(z,s)\text{ is meromorphic on }\mathbb C,\quad
\mathcal E(z,s)=\mathcal E(z,1-s),\quad
\operatorname{Res}_{s=0}\mathcal E=-\tfrac12,\quad
\operatorname{Res}_{s=1}\mathcal E=\tfrac12.}
$$

For the [Kronecker limit formula](../../../modular-function.md#kronecker-limit-formula), evaluate the finite Laurent coefficient at $s=1$. Write $\gamma_E$ for the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant). From $\zeta(u)=1/(u-1)+\gamma_E+O(u-1)$ and $\Gamma'(1/2)/\Gamma(1/2)=-\gamma_E-2\log2$ we obtain

$$
\Xi(2s-1)=\frac1{2(s-1)}+\frac{\gamma_E-\log(4\pi)}2+O(s-1).
$$

The gamma derivative follows by differentiating the [Gamma duplication formula](../../../complex-analysis.md#gamma-duplication-formula) and using $\Gamma'(1)=-\gamma_E$. Multiplication by $y^{1-s}$ adds $-\tfrac12\log y$ to the constant term; the other constant term contributes $\Xi(2)y=\pi y/6$.

The half-order [Modified Bessel function of the second kind](../../../analysis.md#modified-bessel-function-of-the-second-kind) is $K_{1/2}(Y)=\sqrt{\pi/(2Y)}e^{-Y}$. For example, in its even integral representation set $v/2$ as variable and then $u=\sinh(v/2)$: $\cosh v=1+2u^2$ and the $\cosh(v/2)$ factor converts the integral to a Gaussian. At $s=1$ the nonconstant Eisenstein coefficients are consequently $\sigma_{-1}(|r|)e^{-2\pi|r|y}$. On the other hand, the absolutely convergent logarithmic series gives

$$
\log\prod_{n\geq1}(1-q^n)=-\sum_{r\geq1}\sigma_{-1}(r)q^r.
$$

Adding this identity to its conjugate identifies the nonconstant sum as $-2\log|\prod_{n\geq1}(1-q^n)|$. With the analytic [Dedekind eta function](../../../string-theory.md#dedekind-eta-function) product $\eta(z)=q^{1/24}\prod_{n\geq1}(1-q^n)$, the resulting answer is

$$
\boxed{\mathcal E(z,s)=\frac1{2(s-1)}+\frac{\gamma_E-\log(4\pi)}2
-\log\left(\sqrt y\,|\eta(z)|^2\right)+O(s-1).}
$$

This derivation of the [Kronecker limit formula](../../../modular-function.md#kronecker-limit-formula) uses the analytic eta product only; it does not assume its modular transformation. The lattice series is invariant for $\Re s>1$ by an integral change of the pair $(m,n)$ and $\Im(\gamma z)=y/|cz+d|^2$. Analytic continuation preserves this invariance, so its finite Laurent coefficient is invariant too. This supplies the independent weight-two transformation argument used in Question 2.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
