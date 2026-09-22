# Paper 75

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper75.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper75.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The closed [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) is

$$
\boxed{\mathcal F=\{z=x+iy\in\mathbb H:|x|\leq\tfrac12,\ |z|\geq1\}.}
$$

Its vertical sides are paired by $T:z\mapsto z+1$, and its circular sides by $S:z\mapsto-1/z$. It is a fundamental region with boundary identifications. To obtain exactly one representative of each orbit, use $-1/2<x\leq1/2$ and, on $|z|=1$, retain the half with $x\geq0$. We will include both vertices when discussing the closure.

To prove existence of a representative, fix $z\in\mathbb H$. Among primitive integer pairs $(c,d)$ choose one minimizing $|cz+d|$. The minimum exists: below any fixed bound, $|c|y\leq|cz+d|$ bounds $c$, and then the real part bounds $d$, so only finitely many pairs occur. Extend this primitive pair to the bottom row of a determinant-one integer [matrix](../../../vector-space.md#matrix) $\gamma$. Since

$$
\operatorname{Im}(\gamma z)=\frac{y}{|cz+d|^2},
$$

this makes the imaginary part maximal over the orbit. Translate by an integer to put the real part in $[-1/2,1/2]$. If the resulting point had modulus below one, inversion by $S$ would increase its imaginary part, a contradiction. Thus every orbit meets $\mathcal F$.

For uniqueness in the interior, note that $y\geq\sqrt3/2$ throughout $\mathcal F$ and that $|cz+d|\geq1$ for every primitive pair. If $|c|\geq2$, then $|cz+d|\geq|c|y\geq\sqrt3>1$. For $|c|=1$, the minimum over integer $d$ is attained at $d=0$ or, at an endpoint, at a neighboring integer: $|z|\geq1$ and $|z\pm1|^2=|z|^2\pm2x+1\geq1$. All larger $|d|$ give a strict inequality. If $c=0$, primitivity gives $d=\pm1$.

If two points in $\mathcal F$ are equivalent, applying this inequality to the transformation and its inverse shows their imaginary parts are equal. For two interior points equality forces $c=0,d=\pm1$, hence an integer translation. Their real parts lie in an interval of length one, so the translation is zero. The only [matrices](../../../vector-space.md#matrix) acting trivially are $\pm I$. On the boundary, the equality cases give precisely the stated vertical and circular identifications. This establishes the fundamental-domain claim, including its boundary convention.

An [elliptic point of a modular curve](../../../modular-function.md#elliptic-point-of-a-modular-curve) means a fixed point of a nonidentity element of the effective [modular group](../../../modular-function.md#modular-group) $PSL_2(\mathbb Z)$; the central [matrix](../../../vector-space.md#matrix) $-I$ is not counted, since it acts trivially everywhere. The equality cases above show that the only such points in the closed region are

$$
\boxed{i,\qquad \rho=-\tfrac12+\tfrac{\sqrt3}{2}i,\qquad
\rho_+=\tfrac12+\tfrac{\sqrt3}{2}i=\rho+1.}
$$

Their [stabilizer subgroups](../../../group-theory.md#stabilizer-subgroup) in $SL_2(\mathbb Z)$ are

$$
\boxed{\operatorname{Stab}(i)=\langle S\rangle\cong C_4,\quad
\operatorname{Stab}(\rho)=\langle ST\rangle\cong C_6,\quad
\operatorname{Stab}(\rho_+)=\langle TS\rangle\cong C_6,}
$$

where

$$
S=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\quad
ST=\begin{pmatrix}0&-1\\1&1\end{pmatrix},\quad
TS=\begin{pmatrix}1&-1\\1&0\end{pmatrix}.
$$

Indeed $S^2=-I$, $(ST)^3=(TS)^3=-I$, and their fractional-linear fixed-point equations give the listed points. To see that these are the full [stabilizer subgroups](../../../group-theory.md#stabilizer-subgroup), equality in $|cz+d|\geq1$ leaves only bottom rows $(0,\pm1),(\pm1,0)$, with the extra neighboring rows at the vertices. The fixed-point equation then fixes the top row. This yields exactly four [matrices](../../../vector-space.md#matrix) at $i$, six at each vertex, and just $\{\pm I\}$ elsewhere. These are the [elliptic stabilizers of the modular group](../../../modular-function.md#elliptic-stabilizers-of-the-modular-group). After passing to $PSL_2(\mathbb Z)$ their effective orders are two and three. The two vertices represent the same elliptic orbit.

## 2

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Normalize the weight-four and weight-six [Eisenstein series](../../../modular-function.md#eisenstein-series) to have constant term one. Their [Fourier expansions](../../../fourier-series.md) begin

$$
E_4=1+240q+O(q^2),\qquad E_6=1-504q+O(q^2),\qquad q=e^{2\pi iz}.
$$

Their absolutely convergent lattice sums transform by [modular weights](../../../modular-function.md#weight-of-a-modular-form) four and six under reindexing by the [modular group](../../../modular-function.md#modular-group), and their [Fourier expansions](../../../fourier-series.md) prove holomorphy at its [modular cusp](../../../modular-function.md#cusp-of-a-modular-group). Thus they are elements of $M_4,M_6$.

We use the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group): for a nonzero weight-$k$ form,

$$
v_\infty(f)+\tfrac12v_i(f)+\tfrac13v_\rho(f)+\sum_{z\ne i,\rho}v_z(f)=\frac{k}{12}.
$$

The sum uses one point of each ordinary orbit. This is the argument principle on a truncated fundamental region: paired vertical integrals cancel, the circle pairing $f(-1/z)=z^kf(z)$ contributes the [modular weight](../../../modular-function.md#weight-of-a-modular-form) term, and local quotient coordinates at the two [elliptic points of a modular curve](../../../modular-function.md#elliptic-point-of-a-modular-curve) [modular weight](../../../modular-function.md#weight-of-a-modular-form) their orders by $1/2,1/3$. All orders are nonnegative for a holomorphic [modular form](../../../modular-function.md#modular-form).

Define the [modular discriminant](../../../modular-function.md#modular-discriminant) by

$$
\Delta=\frac{E_4^3-E_6^2}{1728}=q+O(q^2).
$$

It is a weight-twelve [cusp form](../../../modular-function.md#cusp-form). Its order at infinity is one, exhausting the valence total $12/12=1$. Hence $\Delta$ has no zeros in $\mathbb H$. Therefore every weight-$k$ [cusp form](../../../modular-function.md#cusp-form) is divisible by $\Delta$, with quotient holomorphic on $\mathbb H$ and at the [modular cusp](../../../modular-function.md#cusp-of-a-modular-group):

$$
\boxed{S_k=\Delta M_{k-12}.}
$$

Negative [modular weights](../../../modular-function.md#weight-of-a-modular-form) vanish by the valence formula, and odd [modular weights](../../../modular-function.md#weight-of-a-modular-form) vanish because $-I$ acts by $(-1)^k$. Weight-zero forms are constant: they descend holomorphically to the [compactified modular curve](../../../modular-function.md#compactified-modular-curve), and the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) applies. There are no weight-two forms: $f(i)=i^2f(i)=-f(i)$ forces a zero at $i$, whose valence contribution $1/2$ exceeds $2/12$.

Every nonnegative even [modular weight](../../../modular-function.md#weight-of-a-modular-form) other than two is $4a+6b$ with $a,b\geq0$. If $k\equiv0\pmod4$, take $b=0$; if $k\equiv2\pmod4$ and $k\geq6$, take $b=1$. For $f\in M_k$, choose such a monomial $h=E_4^aE_6^b$, whose constant term is one. Subtracting the constant term $c$ of $f$ gives $f-ch\in S_k$, so

$$
f=cE_4^aE_6^b+\Delta g,\qquad g\in M_{k-12}.
$$

Induction on [modular weight](../../../modular-function.md#weight-of-a-modular-form), together with $1728\Delta=E_4^3-E_6^2$, proves that every [modular form](../../../modular-function.md#modular-form) is a [polynomial](../../../polynomial.md) in $E_4,E_6$.

For [algebraic independence](../../../algebra.md#algebraic-independence), first fix one [modular weight](../../../modular-function.md#weight-of-a-modular-form) $w$. All solutions of $4a+6b=w$ have the same residue of $a$ modulo three and the same parity of $b$. Consequently their monomials can be written

$$
E_4^{a_0}E_6^{b_0}(E_4^3)^j(E_6^2)^{L-j},\qquad j=0,\ldots,L,
$$

for suitable $a_0,b_0,L$. On an open set where the common factor and $E_6$ are nonzero, a linear relation would give a [polynomial](../../../polynomial.md) relation in

$$
R(z)=\frac{E_4(z)^3}{E_6(z)^2}=1+1728q+O(q^2).
$$

This is nonconstant. By the [open mapping theorem](../../../functional-analysis.md#open-mapping-theorem-functional-analysis), a [polynomial](../../../polynomial.md) vanishing on all its values must be the zero [polynomial](../../../polynomial.md). Thus same-weight monomials are linearly independent.

Different [modular weights](../../../modular-function.md#weight-of-a-modular-form) cannot cancel either. Suppose $\sum_w P_w(E_4,E_6)=0$ with each $P_w$ weighted homogeneous. Transform by $\gamma_n=\begin{pmatrix}1&0\\n&1\end{pmatrix}$. At any fixed $z\in\mathbb H$ this gives

$$
\sum_w(nz+1)^wP_w(E_4(z),E_6(z))=0\qquad(n\in\mathbb Z).
$$

The numbers $nz+1$ are infinitely many distinct values, so the [polynomial](../../../polynomial.md) in that number vanishes identically, and every $P_w(z)=0$. The same-weight independence then sets every [coefficient](../../../vector-space.md#coefficient) to zero. This is the [graded weights separate analytic polynomial relations](../../../modular-function.md#graded-weights-separate-analytic-polynomial-relations) argument. Hence

$$
\boxed{M_*(SL_2(\mathbb Z))\cong\mathbb C[E_4,E_6],\qquad \deg E_4=4,\ \deg E_6=6,}
$$

with **algebraically independent generators**. Multiplying the two [Eisenstein series](../../../modular-function.md#eisenstein-series) by their nonzero lattice-normalization constants does not alter either generation or independence.

## 3

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator) and let $\mathcal M_n$ be all integral [matrices](../../../vector-space.md#matrix) of positive [determinant](../../../linear-algebra.md#determinant) $n$. Their left $SL_2(\mathbb Z)$ cosets have the unique [determinant-n matrix representatives for Hecke operators](../../../modular-function.md#determinant-n-matrix-representatives-for-hecke-operators)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d>0,\ ad=n,\ 0\leq b<d.
$$

Integer row operations reduce the first column to $(a,0)^T$, and a row shear then reduces $b$ modulo $d$. Define

$$
\boxed{T_nf=n^{k/2-1}\sum_{\alpha\in SL_2(\mathbb Z)\backslash\mathcal M_n}f|_k\alpha
=n^{k-1}\sum_{ad=n}d^{-k}\sum_{b=0}^{d-1}f\left(\frac{az+b}{d}\right).}
$$

Changing representatives does not affect the sum, while right multiplication by the [modular group](../../../modular-function.md#modular-group) permutes the cosets. Hence $T_nf$ has the same modular transformation law. Rational positive-determinant slash transforms are holomorphic on $\mathbb H$ and preserve [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) vanishing: choose an integral [matrix](../../../vector-space.md#matrix) carrying infinity to their rational image [modular cusp](../../../modular-function.md#cusp-of-a-modular-group), after which the remaining [matrix](../../../vector-space.md#matrix) is upper triangular. Its positive dilation sends the original decaying [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) expansion to another decaying expansion. Thus these are well-defined [Hecke operators](../../../modular-function.md#hecke-operator) on $S_k$.

For the [Fourier expansion](../../../fourier-series.md), insert $f(z)=\sum_{m\geq1}a(m)e^{2\pi imz}$. The sum over $b$ vanishes unless $d\mid m$, in which case it is $d$. Writing $m=d\ell$, the resulting exponential is $q^{a\ell}$, and its factor is $n^{k-1}d^{1-k}=a^{k-1}$. Therefore

$$
\boxed{a(r;T_nf)=\sum_{a\mid(n,r)}a^{k-1}a(nr/a^2;f).}
$$

In particular, the first [coefficient](../../../vector-space.md#coefficient) of $T_nf$ is $a(n;f)$.

Assume $f\ne0$ is a simultaneous [Hecke eigenform](../../../modular-function.md#hecke-eigenform). The first-coefficient identity gives $a(n)=\lambda(n)a(1)$. If $a(1)=0$, all [coefficients](../../../vector-space.md#coefficient) vanish, contradicting $f\ne0$. After dividing by $a(1)$, we may therefore suppose $a(1)=1$, and then $\lambda(n)=a(n)$.

We derive the relations needed for the [Euler product](../../../analytic-number-theory.md#euler-product). For coprime $m,n$, applying the [coefficient](../../../vector-space.md#coefficient) formula twice splits the divisors into their disjoint prime supports and yields $T_mT_n=T_{mn}$. For one prime define formal Fourier operators $U_p(\sum a(r)q^r)=\sum a(pr)q^r$ and $V_pf(z)=f(pz)$. The [coefficient](../../../vector-space.md#coefficient) formula gives

$$
T_{p^r}=\sum_{j=0}^r p^{j(k-1)}V_p^jU_p^{r-j},\qquad U_pV_p=I.
$$

Multiplying this finite sum by $T_p=U_p+p^{k-1}V_p$ shows that

$$
T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}\qquad(r\geq1).
$$

These auxiliary operators need not separately preserve level one; the identities concern their action on [Fourier series](../../../fourier-series.md). Applied to the eigenform, they give

$$
a(mn)=a(m)a(n)\quad((m,n)=1),\qquad
a(p^{r+1})=a(p)a(p^r)-p^{k-1}a(p^{r-1}).
$$

The prime-power generating function consequently satisfies

$$
\sum_{r\geq0}a(p^r)X^r=\frac1{1-a(p)X+p^{k-1}X^2}.
$$

Multiplicativity and unique [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) now prove the [Euler product of a Hecke eigenform](../../../modular-function.md#euler-product-of-a-hecke-eigenform):

$$
\boxed{L(f,s)=\prod_p\left(1-a(p)p^{-s}+p^{k-1-2s}\right)^{-1}.}
$$

For the original unnormalized form, the right side is multiplied by $a(1)$ and $a(p)$ in the factors is replaced by $\lambda(p)=a(p)/a(1)$. The zero form has $L=0$ and is excluded from the nonzero-eigenform product assertion.

These manipulations initially hold in an absolutely convergent right half-plane. For example, $y^{k/2}|f(z)|$ is bounded by modular invariance and [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) decay. The [coefficient](../../../vector-space.md#coefficient) integral at $y=1/n$ gives $|a(n)|\leq Cn^{k/2}$, so $\operatorname{Re}s>k/2+1$ is sufficient. No analytic continuation is needed to justify the initial product.

## 4

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $d\mu=dx\,dy/y^2$ and distinguish the all-pairs [Eisenstein series](../../../modular-function.md#eisenstein-series) in this problem from its primitive version

$$
E_0(z,w)=\frac12\sum_{(c,d)=1}\frac{y^w}{|cz+d|^{2w}}
=\sum_{\Gamma_\infty\backslash SL_2(\mathbb Z)}(\operatorname{Im}\gamma z)^w.
$$

Separating each nonzero integer pair into a positive integer multiple of a primitive pair gives

$$
E(z,w)=2\pi^{-w}\Gamma(w)\zeta(2w)E_0(z,w).
$$

The factor two accounts for the two signs of a primitive pair. It must not be omitted in the [Rankin–Selberg unfolding](../../../modular-function.md#rankin-selberg-method).

Because $f\overline g y^k$ and $d\mu$ are invariant, unfolding its integral against $E_0$ produces the strip $0\leq x<1$, $y>0$:

$$
\int_{\mathcal F}f(z)\overline{g(z)}y^kE_0(z,w)d\mu
=\int_0^\infty\int_0^1 f(x+iy)\overline{g(x+iy)}y^{w+k-2}dx\,dy.
$$

The $x$ integral of the product [Fourier expansions](../../../fourier-series.md) is $\sum_{n\geq1}a(n)\overline{b(n)}e^{-4\pi ny}$. The [Gamma function](../../../complex-analysis.md#gamma-function) integral then gives

$$
\int_{\mathcal F}f\overline g y^kE_0(z,w)d\mu
=\frac{\Gamma(w+k-1)}{(4\pi)^{w+k-1}}F(w+k-1).
$$

These steps first follow by absolute convergence sufficiently far right. For $f=g$, positive unfolding and [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) decay show the square-coefficient series converges for $\operatorname{Re}s>k$; the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives the same absolute-convergence range for the mixed series.

Put $w=s-k+1$ and define

$$
\boxed{\mathcal R(s):=2\pi^{-w}\Gamma(w)\zeta(2w)\frac{\Gamma(s)}{(4\pi)^s}F(s)
=\int_{\mathcal F}f(z)\overline{g(z)}y^kE(z,w)d\mu.}
$$

This is the [zeta-completed Rankin-Selberg coefficient series](../../../modular-function.md#zeta-completed-rankin-selberg-coefficient-series). Equivalently, solving this formula for $F(s)$ expresses the requested series directly in terms of the all-pairs Eisenstein integral.

The exponential decay of [cusp forms](../../../modular-function.md#cusp-form) at infinity dominates the [polynomial](../../../polynomial.md) growth in $y$ of the [Eisenstein series](../../../modular-function.md#eisenstein-series) and its parameter derivatives, locally uniformly away from its poles. Thus its stated continuation can be passed through the integral. The completed series is meromorphic on $\mathbb C$, with possible simple poles only at $s=k-1,k$, and its [functional equation](../../../analysis.md#functional-equation) is

$$
\boxed{\mathcal R(s)=\mathcal R(2k-1-s).}
$$

Indeed $w\mapsto1-w$ corresponds to $s\mapsto2k-1-s$. If $\langle f,g\rangle=0$, both pole residues vanish and the completion is entire.

The normalization of the poles can also be made explicit. The constant term of the given [Eisenstein series](../../../modular-function.md#eisenstein-series) is

$$
2\pi^{-w}\Gamma(w)\zeta(2w)y^w
+2\pi^{1/2-w}\Gamma(w-\tfrac12)\zeta(2w-1)y^{1-w}.
$$

The second term has residue one at $w=1$, since the pole of $\zeta(2w-1)$ has residue $1/2$; the [functional equation](../../../analysis.md#functional-equation) gives residue minus one at $w=0$. Hence the residues of $\mathcal R$ at $k$ and $k-1$ are respectively $\langle f,g\rangle$ and $-\langle f,g\rangle$, the [Petersson inner product](../../../modular-function.md#petersson-inner-product).

It is important to separate this completed statement from the raw $F$. Inverting the completion gives [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) of $F$, but zeros of $\zeta(2s-2k+2)$ in the denominator can give additional possible poles unless canceled by the integral. Nor does $F$ itself satisfy the unweighted symmetry $s\leftrightarrow2k-1-s$. At the two displayed completion poles, for a nontrivial [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) [modular weight](../../../modular-function.md#weight-of-a-modular-form),

$$
\boxed{\operatorname*{Res}_{s=k}F(s)=\frac{3(4\pi)^k}{\pi\Gamma(k)}\langle f,g\rangle,
\qquad F(k-1)=\frac{(4\pi)^{k-1}}{\Gamma(k-1)}\langle f,g\rangle.}
$$

The latter is finite because the pole of $\Gamma(w)$ cancels that of the integral at $w=0$, using $\zeta(0)=-1/2$. In particular, taking $f=g\ne0$ gives a raw-series pole at $k$ and regularity at $k-1$. The direct analogue of the stipulated two-pole Eisenstein properties is therefore the completed function $\mathcal R$, not the raw series with all completion factors suppressed.

Finally suppose the two $L$-series have [Euler products](../../../analytic-number-theory.md#euler-product). With first [coefficients](../../../vector-space.md#coefficient) normalized to one, their [coefficients](../../../vector-space.md#coefficient) are multiplicative, so $a(n)\overline{b(n)}$ is multiplicative too. Therefore

$$
\boxed{F(s)=\prod_p\left(\sum_{r\geq0}a(p^r)\overline{b(p^r)}p^{-rs}\right),}
$$

initially in its absolute-convergence half-plane. For unnormalized forms multiply the product by $a(1)\overline{b(1)}$ and use normalized [coefficients](../../../vector-space.md#coefficient) inside it.

For the usual degree-two Hecke products of Question 3, take roots $\alpha_p,\beta_p$ with sum $a(p)$ and product $p^{k-1}$, and $\gamma_p,\delta_p$ with sum $b(p)$ and the same product. The prime-power recurrence gives $a(p^r)=(\alpha_p^{r+1}-\beta_p^{r+1})/(\alpha_p-\beta_p)$ and the analogous expression for $b$. Multiplying and summing four geometric series proves the [Euler factor of a coefficientwise product of Hecke eigenforms](../../../modular-function.md#euler-factor-of-a-coefficientwise-product-of-hecke-eigenforms):

$$
\boxed{F_p(X)=\frac{1-p^{2k-2}X^2}
{(1-\alpha_p\overline\gamma_pX)(1-\alpha_p\overline\delta_pX)
(1-\beta_p\overline\gamma_pX)(1-\beta_p\overline\delta_pX)},\qquad X=p^{-s}.}
$$

Repeated roots are handled by continuity, or directly by the recurrence. Multiplication by $\zeta(2s-2k+2)$ cancels the local numerators and yields the degree-four convolution product. This also explains why the zeta factor belongs in the natural analytic completion.

## 5

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $\mu_N=[PSL_2(\mathbb Z):\overline{\Gamma(N)}]$, where the bar denotes the effective projective image. This is the degree of the [modular curve](../../../modular-function.md#modular-curve) projection, rather than the full $SL_2$ index when $-I$ is not in $\Gamma(N)$.

Reduction modulo $N$ is onto $SL_2(\mathbb Z/N\mathbb Z)$. One proof uses the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) and elementary [matrices](../../../vector-space.md#matrix): over $\mathbb Z/p^r\mathbb Z$, a unimodular first column has a unit entry, so elementary row operations reduce a determinant-one [matrix](../../../vector-space.md#matrix) to the identity. Each elementary [matrix](../../../vector-space.md#matrix) lifts integrally. Over $\mathbb F_p$, the first column has $p^2-1$ choices and the second has $p$ choices with prescribed [determinant](../../../linear-algebra.md#determinant), giving $p(p^2-1)$. Each subsequent prime-power lift has $p^3$ choices, because the determinant-one linearized condition is one trace equation on four entries. Hence

$$
[SL_2(\mathbb Z):\Gamma(N)]=N^3\prod_{p\mid N}(1-p^{-2}).
$$

For $N=1,2$, the subgroup contains $-I$; for $N\geq3$ it does not. Consequently

$$
\mu_1=1,\qquad\mu_2=6,\qquad
\mu_N=\frac{N^3}{2}\prod_{p\mid N}(1-p^{-2})\quad(N\geq3).
$$

For $N\geq2$ there are no effective elliptic [stabilizer subgroups](../../../group-theory.md#stabilizer-subgroup) in the subgroup. Indeed, write $\gamma=I+NB\in\Gamma(N)$. The [determinant](../../../linear-algebra.md#determinant) condition gives $\operatorname{tr}\gamma=2-N^2\det B$. A noncentral elliptic element in $SL_2(\mathbb Z)$ has trace $-1,0$ or $1$, none congruent to $2$ modulo $N^2$ for $N\geq2$. Thus the projective action is torsion-free.

All [cusp widths](../../../modular-function.md#width-of-a-cusp) are $N$. At infinity, $T^h$ lies in the effective subgroup exactly when $h$ is divisible by $N$: the alternative $T^h\equiv-I\pmod N$ can only occur for $N=1,2$, and for $N=2$ it imposes the same condition. Every rational [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) is a modular translate of infinity, and the subgroup is normal, so the same width holds there. The sum of [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) [analytic ramification indices](../../../complex-analysis.md#ramification-index-of-a-holomorphic-map) equals $\mu_N$, giving $\mu_N/N$ [modular cusps](../../../modular-function.md#cusp-of-a-modular-group).

The base $X(1)$ is a sphere. For instance $j=E_4^3/\Delta$ is a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) on it with a single simple pole at the [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) and no other poles, using the nonvanishing of $\Delta$ proved above. It therefore defines a degree-one map to the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), making the base [genus](../../../topology.md#genus-of-a-surface) zero.

The only branch values of $X(N)\to X(1)$ are the two elliptic orbits and the [modular cusp](../../../modular-function.md#cusp-of-a-modular-group). For $N\geq2$, the numbers of points above them and their [analytic ramification indices](../../../complex-analysis.md#ramification-index-of-a-holomorphic-map) are respectively $\mu_N/2$ with index two, $\mu_N/3$ with index three, and $\mu_N/N$ with index $N$. Applying the [Riemann-Hurwitz formula](../../../complex-analysis.md#riemann-hurwitz-formula) directly,

$$
\begin{aligned}
2g(X(N))-2
&=-2\mu_N+\frac{\mu_N}{2}(2-1)+\frac{\mu_N}{3}(3-1)+\frac{\mu_N}{N}(N-1)\\
&=\mu_N\left(\frac16-\frac1N\right).
\end{aligned}
$$

This is the [elliptic and cusp ramification for principal level](../../../modular-function.md#elliptic-and-cusp-ramification-for-principal-level) calculation. Level one is the identity projection. The complete result is

$$
\boxed{g(X(1))=g(X(2))=0,\qquad
g(X(N))=1+\frac{N^2(N-6)}{24}\prod_{p\mid N}(1-p^{-2})\quad(N\geq3).}
$$

For example the genera for $N=3,4,5,6,7$ are $0,0,0,1,3$. Keeping the exceptional projective index at level two is essential; applying the factor one-half there would give a nonintegral answer. This agrees with the [principal congruence modular curve genus](../../../modular-function.md#principal-congruence-modular-curve-genus) formula obtained from these branch counts.

## 6

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Write $U_u=\begin{pmatrix}1&u/D\\0&1\end{pmatrix}$ and $\tau(\chi)=\sum_{u\bmod D}\chi(u)e^{2\pi iu/D}$. The [finite Fourier transform of a primitive Dirichlet character](../../../algebraic-number-theory.md#finite-fourier-transform-of-a-primitive-dirichlet-character) gives

$$
\sum_{u\bmod D}\overline\chi(u)e^{2\pi inu/D}=\chi(n)\tau(\overline\chi).
$$

For $(n,D)=1$ this follows by multiplying residues by $n$. For a nonunit $n$, primitivity supplies a unit $v\equiv1\pmod{D/p}$ with nontrivial character value, for a prime $p\mid(n,D)$; multiplication by $v$ leaves the exponential unchanged and forces the sum to vanish. Orthogonality of the finite exponentials gives $\sum_{n\bmod D}|\sum_u\chi(u)e^{2\pi inu/D}|^2=D\sum_u|\chi(u)|^2=D\varphi(D)$. The primitive transform identity makes the left side $\varphi(D)|\tau(\chi)|^2$. Thus the primitive [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) is nonzero, with $|\tau(\chi)|^2=D$. Consequently the twist is the finite rational-translation sum

$$
\boxed{f_\chi=\frac1{\tau(\overline\chi)}\sum_{u\bmod D}\overline\chi(u)f|_kU_u.}
$$

This representation will prove both the level statement and the Fricke formula.

Take $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(ND^2)$, and choose $v\equiv d^2u\pmod D$. Since $ad\equiv1\pmod D$, this means $av\equiv ud\pmod D$. Direct multiplication gives

$$
U_u\gamma U_v^{-1}
=\begin{pmatrix}
a+uc/D&b+(ud-av)/D-ucv/D^2\\
c&d-cv/D
\end{pmatrix}=:\gamma_u.
$$

Every entry is integral, its [determinant](../../../linear-algebra.md#determinant) is one, and its lower-left entry is divisible by $N$. Thus $\gamma_u\in\Gamma_0(N)$. Its lower-right entry is congruent to $d$ modulo $N$, so $f|\gamma_u=\psi(d)f$ by its [nebentypus character](../../../modular-function.md#nebentypus-character). Using the right-action property of the slash operator,

$$
f_\chi|\gamma=\frac{\psi(d)}{\tau(\overline\chi)}
\sum_u\overline\chi(u)f|U_v.
$$

The map $u\mapsto v=d^2u$ permutes the residue classes. Reindexing gives $\overline\chi(u)=\chi(d)^2\overline\chi(v)$, so

$$
\boxed{f_\chi|_k\gamma=\psi(d)\chi(d)^2f_\chi.}
$$

This proves the required [modular weight](../../../modular-function.md#weight-of-a-modular-form) and character on $\Gamma_0(ND^2)$.

Cuspidality must also be checked. For any [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) [matrix](../../../vector-space.md#matrix) $\sigma\in SL_2(\mathbb Z)$ and any rational translation $U_u$, choose $\rho\in SL_2(\mathbb Z)$ with $\rho\infty=U_u\sigma\infty$. Then $\rho^{-1}U_u\sigma$ is upper triangular with positive dilation. Since $f|\rho$ decays exponentially at infinity, so does $f|U_u\sigma$. The finite sum defining $f_\chi$ therefore tends to zero at every [modular cusp](../../../modular-function.md#cusp-of-a-modular-group); its transformation law supplies a [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) period, so its holomorphic [Fourier expansion](../../../fourier-series.md) has zero constant term there. Hence the [primitive twist at coprime level](../../../modular-function.md#primitive-twist-at-coprime-level) is

$$
\boxed{f_\chi\in S_k(\Gamma_0(ND^2),\psi\chi^2).}
$$

Now put $W_M=\begin{pmatrix}0&-1\\M&0\end{pmatrix}$ and $g=f|_kW_N$, always using the [determinant](../../../linear-algebra.md#determinant) factor specified in the question. For each unit $u$ choose a unit $v$ with $Nuv\equiv-1\pmod D$, possible because $(N,D)=1$. The crucial integral [matrix](../../../vector-space.md#matrix) factorization is

$$
\boxed{U_uW_{ND^2}=D\gamma_uW_NU_v,\qquad
\gamma_u=\begin{pmatrix}(1+Nuv)/D&u\\Nv&D\end{pmatrix}\in\Gamma_0(N).}
$$

The right side multiplies out to $\begin{pmatrix}uND&-1\\ND^2&0\end{pmatrix}$, so the identity is exact. Its determinant-one [matrix](../../../vector-space.md#matrix) has lower-right entry $D$, and therefore $f|\gamma_u=\psi(D)f$. A positive scalar [matrix](../../../vector-space.md#matrix) $DI$ acts trivially under the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator), since its [determinant](../../../linear-algebra.md#determinant) contributes $D^k$ and its denominator contributes $D^{-k}$. Thus

$$
f_\chi|W_{ND^2}=\frac{\psi(D)}{\tau(\overline\chi)}\sum_u\overline\chi(u)g|U_v.
$$

The inverse-residue substitution is $u\equiv-(Nv)^{-1}\pmod D$, giving $\overline\chi(u)=\chi(-N)\chi(v)$. The sum over $v$ is $\tau(\chi)g_{\overline\chi}$. Hence the [Fricke transform of a primitive coprime twist](../../../modular-function.md#fricke-transform-of-a-primitive-coprime-twist) is

$$
\boxed{f_\chi|_kW_{ND^2}=\psi(D)\chi(-N)\frac{\tau(\chi)}{\tau(\overline\chi)}\,g_{\overline\chi}
=\psi(D)\chi(N)\frac{\tau(\chi)^2}{D}\,g_{\overline\chi}.}
$$

The second version uses $\tau(\chi)\tau(\overline\chi)=\chi(-1)D$, which follows from $\overline{\tau(\chi)}=\chi(-1)\tau(\overline\chi)$ and $|\tau(\chi)|^2=D$. Here $g_{\overline\chi}=\sum b(n)\overline\chi(n)q^n$ if $g=\sum b(n)q^n$; it is not the complex conjugate function $\overline g$. The coprimality of $N,D$ is used both in the [matrix](../../../vector-space.md#matrix) factorization and in evaluating $\psi(D)$. For $D=1$ the twist is trivial and the formula simply reads $f|W_N=g$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
