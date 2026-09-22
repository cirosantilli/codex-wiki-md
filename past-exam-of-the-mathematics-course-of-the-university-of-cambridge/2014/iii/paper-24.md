# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_24.pdf)

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
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is a map $|\cdot|:K\to\mathbb R_{\geq0}$ satisfying

$$
|x|=0\Longleftrightarrow x=0,\qquad |xy|=|x||y|,\qquad |x+y|\leq|x|+|y|.
$$

A [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value) satisfies the stronger [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) $|x+y|\leq\max(|x|,|y|)$. Two [equivalent absolute values](../../../arithmetic.md#equivalent-absolute-values) induce the same [topology](../../../topology.md), or equivalently differ by a positive real power. The trivial [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) takes value one on every nonzero element. The rational classification and the compactness criterion below concern nontrivial [absolute values on a field](../../../arithmetic.md#absolute-value-algebra); the trivial exceptions are given explicitly.

Here the additive [valuation](../../../algebra.md#valuation) has real values. For any $c>1$, the mutually inverse constructions are

$$
v(x)=-\log_c|x|,\quad v(0)=+\infty,\qquad |x|=c^{-v(x)}.
$$

Multiplicativity becomes $v(xy)=v(x)+v(y)$, and the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) becomes $v(x+y)\geq\min(v(x),v(y))$. Equivalent real-valued [valuations](../../../algebra.md#valuation) differ by positive scaling, so these constructions give the required **bijection on equivalence classes**. Changing $c$ merely rescales the [valuation](../../../algebra.md#valuation).

To justify the topology formulation, $|a|<1$ is equivalent to $a^n\to0$. Thus two nontrivial [absolute values on a field](../../../arithmetic.md#absolute-value-algebra) with the same [topology](../../../topology.md) give the same strict positivity relation on their additive [valuations](../../../algebra.md#valuation). Fix $t$ with $v_1(t)>0$. Comparing the signs of $m v_j(t)-n v_j(x)=v_j(t^m x^{-n})$, for integers $m$ and positive integers $n$, shows that $v_1(x)/v_1(t)$ and $v_2(x)/v_2(t)$ have identical rational cuts. They are equal, proving $v_2=c v_1$ for $c>0$. If one allows [valuations](../../../algebra.md#valuation) in arbitrary ordered groups, the nontrivial classes arising this way are precisely [rank-one valuations](../../../algebra.md#rank-one-valuation): higher-rank ordered value groups do not embed order-preservingly in $\mathbb R$.

For a nontrivial [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value) on $\mathbb Q$, $|n|\leq1$ for every integer $n$, by repeatedly applying the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) to sums of ones. Some prime $p$ must have $|p|<1$, otherwise [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) and multiplicativity would make every nonzero rational have value one. There is at most one such prime: if both $|p|,|q|<1$, a [Bezout identity](../../../algebra.md#bezout-identity) $a p+b q=1$ contradicts the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality). If $p\nmid m$, another [Bezout identity](../../../algebra.md#bezout-identity) gives $|m|=1$. Hence

$$
\boxed{|x|=|p|^{v_p(x)}=|x|_p^{\alpha},\qquad \alpha=-\frac{\log|p|}{\log p}>0.}
$$

This proves the non-Archimedean part of the [Ostrowski theorem](../../../arithmetic.md#ostrowski-s-theorem). If the trivial [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is admitted, it supplies one additional class and is not equivalent to any [p-adic absolute value](../../../arithmetic.md#p-adic-absolute-value).

The [valuation ring](../../../commutative-algebra.md#valuation-ring), its [maximal ideal](../../../commutative-algebra.md#maximal-ideal), and its [residue field](../../../commutative-algebra.md#residue-field) are

$$
R=\{x:|x|\leq1\},\qquad\mathfrak m=\{x:|x|<1\},\qquad k=R/\mathfrak m.
$$

Suppose the [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is nontrivial and $R$ is [compact](../../../topology.md#compact-space). The ideal $\mathfrak m$ is an open additive subgroup of $R$, so $k$ is discrete; as a continuous image of a [compact](../../../topology.md#compact-space) space it is finite. The subgroup $\mathfrak m$ is also closed, since all its cosets are open, and is therefore [compact](../../../topology.md#compact-space). The continuous function $|\cdot|$ attains a maximum $\rho$ on $\mathfrak m$, with $0<\rho<1$. Choose $\pi$ with $|\pi|=\rho$. Then the positive values of $v=-\log|\cdot|$ have least element $-\log\rho$. Division with remainder in this additive subgroup of $\mathbb R$ proves $v(K^\times)=v(\pi)\mathbb Z$. Thus $K$ is a [discretely valued field](../../../commutative-algebra.md#discretely-valued-field) and $\pi$ is a [uniformizer](../../../commutative-algebra.md#uniformizer).

Conversely, normalize the [discrete valuation](../../../commutative-algebra.md#discrete-valuation) by $v(\pi)=1$. If $k$ has $q$ elements, $R/\pi^N R$ has $q^N$ elements. Each quotient therefore supplies a finite cover by balls of radius tending to zero. The ring $R$ is a closed subset of the complete metric field $K$, hence complete and [totally bounded](../../../topological-analysis.md#totally-bounded-space), so it is [compact](../../../topology.md#compact-space). Equivalently,

$$
\boxed{R\cong\varprojlim_N R/\pi^N R,\qquad R\text{ compact}\Longleftrightarrow v(K^\times)\text{ discrete and }|k|<\infty.}
$$

This is the [local compactness criterion for a complete non-Archimedean field](../../../arithmetic.md#local-compactness-criterion-for-a-complete-non-archimedean-field), with nontriviality understood. For the trivial [absolute value on a field](../../../arithmetic.md#absolute-value-algebra), $R=K$ has the discrete [topology](../../../topology.md) and is [compact](../../../topology.md#compact-space) exactly when $K$ is a finite [field](../../../algebra.md#field); its value group is zero rather than a nonzero discrete cyclic group.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [inverse different](../../../arithmetic.md#inverse-different) is the [trace-dual lattice](../../../algebraic-number-theory.md#trace-dual-lattice)

$$
\mathfrak D_{L/K}^{-1}=\{a\in L:\operatorname{Tr}_{L/K}(a\mathcal O_L)\subseteq\mathcal O_K\}.
$$

The integral closure $\mathcal O_L$ is finite free over the complete [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) $\mathcal O_K$. Choose an integral basis and use the nondegenerate [trace pairing](../../../algebraic-number-theory.md#trace-pairing) to form its dual basis over $K$. This exhibits $\mathfrak D^{-1}$ as a full, finite $\mathcal O_K$-lattice. It is stable under multiplication by $\mathcal O_L$, because $b\mathcal O_L\subseteq\mathcal O_L$ for $b\in\mathcal O_L$, and bounded denominators make it a [fractional ideal](../../../commutative-algebra.md#fractional-ideal) of $\mathcal O_L$. Integral elements have integral [field traces](../../../algebraic-number-theory.md#field-trace), so $\mathcal O_L\subseteq\mathfrak D^{-1}$. A nonzero [fractional ideal](../../../commutative-algebra.md#fractional-ideal) of a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) is invertible; its inverse is consequently an integral [ideal](../../../commutative-algebra.md#ideal), the [different ideal](../../../arithmetic.md#different-ideal) $\mathfrak D_{L/K}$.

Assume now $A=\mathcal O_K[x]=\mathcal O_L$, with monic separable [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $g$ of degree $n$. [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) at its distinct roots gives

$$
\operatorname{Tr}_{L/K}\!\left(\frac{x^j}{g'(x)}\right)=\begin{cases}0&0\leq j<n-1,\\1&j=n-1.\end{cases}
$$

Indeed, these are the leading coefficients in the interpolation formula for $X^j$. For any element of $A$, this trace is the coefficient of $X^{n-1}$ in its degree-less-than-$n$ representative modulo $g$. The resulting pairing on the basis $1,x,\ldots,x^{n-1}$ is integral and unimodular: reversing the order of one basis makes its matrix triangular with diagonal ones, since entries vanish when the exponent sum is less than $n-1$. Thus it identifies $A$ with its full $\mathcal O_K$-dual. Translating back to the [trace pairing](../../../algebraic-number-theory.md#trace-pairing) proves

$$
\boxed{\mathfrak D_{L/K}^{-1}=g'(x)^{-1}\mathcal O_L,\qquad\mathfrak D_{L/K}=g'(x)\mathcal O_L.}
$$

For a [totally ramified extension](../../../arithmetic.md#totally-ramified-extension) of degree $n$, any [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi_L$ is an [Eisenstein generator of a totally ramified extension](../../../arithmetic.md#eisenstein-generator-of-a-totally-ramified-extension), and $\mathcal O_L=\mathcal O_K[\pi_L]$. To see the latter equality, use the common [residue field](../../../commutative-algebra.md#residue-field) to expand an integral element in powers of $\pi_L$ with digits from $\mathcal O_K$; reduce powers using its [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) and take limits in the finite complete $\mathcal O_K$-module generated by $1,\pi_L,\ldots,\pi_L^{n-1}$. Write that polynomial as $X^n+\sum_{j<n}a_jX^j$, with $v_L(a_j)\geq n$ for $j<n$. When $p\nmid n$, the derivative's leading term has [valuation](../../../algebra.md#valuation) $n-1$, while every other nonzero derivative term has [valuation](../../../algebra.md#valuation) at least $n$. There can be no cancellation of the unique smallest term. Therefore

$$
\boxed{\mathfrak D_{L/K}=\pi_L^{n-1}\mathcal O_L.}
$$

For the prime-power [p-adic cyclotomic extension](../../../arithmetic.md#cyclotomic-extension-of-a-p-adic-field), put $\zeta=\zeta_{p^r}$ and $e=p^{r-1}(p-1)$. Modulo $p$, the shifted [cyclotomic polynomial](../../../galois-theory.md#cyclotomic-polynomial) $\Phi_{p^r}(1+T)$ is $T^e$, while its constant term is $p$, not a multiple of $p^2$. It is therefore [Eisenstein](../../../commutative-algebra.md#eisenstein-criterion), so $\pi=\zeta-1$ is a [uniformizer](../../../commutative-algebra.md#uniformizer) and $\mathcal O_{K_r}=\mathbb Z_p[\zeta]$. From

$$
\Phi_{p^r}(X)=\frac{X^{p^r}-1}{X^{p^{r-1}}-1}
$$

we obtain, by differentiating the numerator at $\zeta$,

$$
\Phi'_{p^r}(\zeta)=\frac{p^r\zeta^{-1}}{\zeta^{p^{r-1}}-1}.
$$

The denominator is a primitive-$p$ [root of unity](../../../algebra.md#root-of-unity) minus one and has $K_r$-[valuation](../../../algebra.md#valuation) $p^{r-1}$. The [different exponent](../../../arithmetic.md#different-exponent) is consequently $r e-p^{r-1}$, giving

$$
\boxed{\mathfrak D_{K_r/\mathbb Q_p}=(\zeta-1)^{p^{r-1}(r(p-1)-1)}\mathcal O_{K_r}.}
$$

This includes $p=2,r=1$: the extension is trivial and its [different exponent](../../../arithmetic.md#different-exponent) is zero.

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The geometric sum gives

$$
\frac{1-\zeta_p^i}{1-\zeta_p}=1+\zeta_p+\cdots+\zeta_p^{i-1}\equiv i\pmod{\pi_K}.
$$

Since $\Phi_p(1)=p$, its factorization at the nonidentity $p$th [roots of unity](../../../algebra.md#root-of-unity) yields

$$
p=\prod_{i=1}^{p-1}(1-\zeta_p^i)=\pi_K^{p-1}w,\qquad w=\prod_{i=1}^{p-1}\frac{1-\zeta_p^i}{1-\zeta_p}.
$$

Each factor is a [unit](../../../algebra.md#unit-in-a-ring), and [Wilson theorem](../../../number-theory.md#wilson-s-theorem) gives $w\equiv(p-1)!\equiv-1\pmod{\pi_K}$. Set $u=-w^{-1}$. Then $u$ is a [principal unit](../../../arithmetic.md#principal-unit) and

$$
\boxed{\pi_K^{p-1}=-p u,\qquad u\in1+\pi_K\mathcal O_K.}
$$

The minus sign comes from the product of the nonzero elements of the [residue field](../../../commutative-algebra.md#residue-field), not from an arbitrary choice of [uniformizer](../../../commutative-algebra.md#uniformizer).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a [principal unit](../../../arithmetic.md#principal-unit) $u$, apply the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) to $F(T)=T^{p-1}-u$. The residue class one is a root, and $F'(1)=p-1$ is a [unit](../../../algebra.md#unit-in-a-ring). Thus there is a unique $v\in1+\pi_K\mathcal O_K$ with

$$
\boxed{v^{p-1}=u.}
$$

In particular it is a [unit](../../../algebra.md#unit-in-a-ring) of $\mathcal O_K$. Choose this $v$ for the $u$ just obtained and put $\alpha=\pi_K/v$. Then $\alpha^{p-1}=-p$, so $\mathbb Q_p(\alpha)\subseteq K$. The polynomial $T^{p-1}+p$ is [Eisenstein](../../../commutative-algebra.md#eisenstein-criterion), giving degree $p-1$ for the left-hand field. The [p-adic cyclotomic extension](../../../arithmetic.md#cyclotomic-extension-of-a-p-adic-field) $K$ also has degree $p-1$, so

$$
\boxed{K=\mathbb Q_p\!\left(\sqrt[p-1]{-p}\right).}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Choose $\beta$ with $\beta^{p(p-1)}=-p$ and put $N=p(p-1)$. The [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) $T^N+p$ shows that $L=\mathbb Q_p(\beta)$ has degree $N$, is [totally ramified](../../../arithmetic.md#totally-ramified-extension), and has [uniformizer](../../../commutative-algebra.md#uniformizer) $\beta$. Its subfield $\mathbb Q_p(\beta^p)$ is the field $K$ from the previous part. Because $p$ is odd,

$$
a=-\beta^{p-1}\quad\text{satisfies}\quad a^p=p.
$$

Thus $L$ contains $a$ and $\zeta_p$, and contains all roots $a\zeta_p^j$ of $T^p-p$. Conversely $[\mathbb Q_p(a):\mathbb Q_p]=p$, while $[K:\mathbb Q_p]=p-1$. Their coprime degrees force their compositum to have degree $N$. It is contained in $L$ and hence equals it. Therefore **$L$ is exactly the splitting field**, not merely an extension containing it.

The [Galois group](../../../galois-theory.md#galois-group) has a normal subgroup $H=\operatorname{Gal}(L/K)$ of order $p$, acting by $\beta\mapsto\zeta_p^j\beta$. The $(p-1)$st [roots of unity](../../../algebra.md#root-of-unity) already lie in $\mathbb Q_p$ by the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma). The maps $\beta\mapsto\omega\beta$, with $\omega^{p-1}=1$, supply a complement of order $p-1$. Its conjugation acts faithfully on $H$, so $G\cong C_p\rtimes\mathbb F_p^\times$.

Normalize $v_L(\beta)=1$. Total ramification and the [uniformizer criterion for lower ramification groups](../../../arithmetic.md#uniformizer-criterion-for-lower-ramification-groups) reduce the calculation to $i_G(\sigma)=v_L(\sigma\beta-\beta)$. For nonidentity $\sigma\in H$,

$$
i_G(\sigma)=1+v_L(\zeta_p^j-1)=1+p,
$$

since $e(L/K)=p$ and $v_K(\zeta_p^j-1)=1$. For $\sigma\notin H$, write $\sigma\beta=\omega\zeta_p^j\beta$ with $\omega\ne1$. Its multiplier has residue $\overline\omega\ne1$, so $i_G(\sigma)=1$. The [lower ramification numbering](../../../arithmetic.md#lower-ramification-numbering) is therefore

$$
\boxed{G_{-1}=G_0=G,\qquad G_1=\cdots=G_p=H\cong C_p,\qquad G_{p+1}=1.}
$$

All later groups are trivial. The wild lower break is $p$, not one. In the [upper ramification numbering](../../../arithmetic.md#upper-ramification-numbering), the [Herbrand function](../../../arithmetic.md#herbrand-function) sends this break to $p/(p-1)$: $G^0=G$, $G^u=H$ for $0<u\leq p/(p-1)$, and $G^u=1$ above it.

As an independent consistency check, the [different exponent from ramification groups](../../../arithmetic.md#different-exponent-from-ramification-groups) is $(N-1)+p(p-1)=2N-1$. The derivative of the [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) gives the same answer, $v_L(N\beta^{N-1})=N+(N-1)$, since $v_L(p)=N$.

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [idele group](../../../algebraic-number-theory.md#idele-group) is the multiplicative [restricted product](../../../algebraic-number-theory.md#restricted-product)

$$
J_K=\prod_v'K_v^\times
$$

with respect to $\mathcal O_v^\times$ at the finite [places of a number field](../../../algebraic-number-theory.md#place-of-a-number-field); $K_v$ is the [completion of a valued field](../../../arithmetic.md#completion-of-a-valued-field) at the place $v$. Thus each tuple has nonzero components, and all but finitely many finite components are [units](../../../algebra.md#unit-in-a-ring). Its [restricted product topology on the idele group](../../../algebraic-number-theory.md#restricted-product-topology-on-the-idele-group) has basic open sets $\prod_{v\in S}W_v\times\prod_{v\notin S}\mathcal O_v^\times$, where $S$ is finite and contains the infinite places, and each $W_v$ is open in $K_v^\times$. In particular $U_K$ is an open subgroup.

Embed $K^\times$ diagonally. Take a neighbourhood of one whose finite components all lie in $\mathcal O_v^\times$ and whose infinite components satisfy $|x_v-1|<1/2$ in the usual real or complex modulus. A diagonal element there is an algebraic [unit](../../../algebra.md#unit-in-a-ring) $a$. If $a\ne1$, then $a-1$ is a nonzero [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer), so its [field norm](../../../algebraic-number-theory.md#field-norm) is a nonzero integer. But

$$
0<|N_{K/\mathbb Q}(a-1)|=\prod_{\sigma\text{ real}}|\sigma(a)-1|\prod_{\sigma\text{ complex}}|\sigma(a)-1|^2<1,
$$

a contradiction. Thus **$K^\times$ is discrete**. It is also closed: in a topological group, a subgroup with an isolated identity cannot have an external accumulation point, since quotients of two nearby subgroup elements would approach the identity.

Send an [idele](../../../algebraic-number-theory.md#idele) to its associated [fractional ideal](../../../commutative-algebra.md#fractional-ideal) by

$$
I(x)=\prod_{v\text{ finite}}\mathfrak p_v^{\operatorname{ord}_v(x_v)}.
$$

Only finitely many exponents are nonzero. This homomorphism is onto, by choosing powers of local [uniformizers](../../../commutative-algebra.md#uniformizer), and its kernel is $U_K$. Diagonal elements map to [principal fractional ideals](../../../commutative-algebra.md#principal-fractional-ideal). The resulting quotient gives

$$
\boxed{J_K/(K^\times U_K)\cong\operatorname{Cl}(K).}
$$

It is a topological isomorphism when the [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) is given the discrete [topology](../../../topology.md), since $U_K$ is open.

Use normalized local moduli: real modulus, squared complex modulus, and $|\pi_v|_v=(N\mathfrak p_v)^{-1}$ at a finite place. The [idelic modulus](../../../algebraic-number-theory.md#idelic-modulus) $\|x\|=\prod_v|x_v|_v$ defines $J_K^1=\ker\|\cdot\|$, the [norm-one idele group](../../../algebraic-number-theory.md#norm-one-idele-group). The [product formula](../../../algebraic-number-theory.md#product-formula) puts $K^\times$ inside this kernel. Every ideal class has a representative in $J_K^1$, because an infinite component can be rescaled to correct the modulus without altering its [fractional ideal](../../../commutative-algebra.md#fractional-ideal). The compact space $J_K^1/K^\times$ therefore maps continuously onto the discrete [ideal class group](../../../algebraic-number-theory.md#ideal-class-group). Its image must be finite, proving **$\operatorname{Cl}(K)$ is finite**.

For the [Dirichlet unit theorem](../../../algebraic-number-theory.md#dirichlet-s-unit-theorem), put $U^1=U_K\cap J_K^1$ and $E=K^\times\cap U^1=\mathcal O_K^\times$. Let $r_1$ count real embeddings and $r_2$ count conjugate complex pairs. Infinite logarithms define a continuous surjection

$$
\ell:U^1\longrightarrow H=\{(t_1,\ldots,t_{r_1+r_2})\in\mathbb R^{r_1+r_2}:\sum_i t_i=0\},
$$

using $\log|x_v|$ at real places and $2\log|x_v|$ at complex places. Its kernel is [compact](../../../topology.md#compact-space): it consists of real signs, complex unit circles, and the product of compact finite-place unit groups. More generally the inverse image of a bounded closed subset of $H$ is [compact](../../../topology.md#compact-space). Since $E$ is closed and discrete, its intersection with each such inverse image is finite. Hence $\Lambda=\ell(E)$ is discrete in $H$, and the kernel $E\cap\ker\ell$ is a finite group. It is exactly the [roots of unity](../../../algebra.md#root-of-unity) $\mu(K)$, since every element of a finite multiplicative group has finite order and every [root of unity](../../../algebra.md#root-of-unity) has all local moduli one.

The image of $U^1$ in $J_K^1/K^\times$ is an open subgroup, hence also closed, and is homeomorphic to $U^1/E$. The assumed compactness therefore makes $U^1/E$ [compact](../../../topology.md#compact-space), and its continuous quotient $H/\Lambda$ is [compact](../../../topology.md#compact-space). A discrete cocompact subgroup of a real [vector space](../../../vector-space.md) is a full [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice), of rank $\dim H=r_1+r_2-1$. Thus $E/\mu(K)\cong\mathbb Z^{r_1+r_2-1}$, and lifting a lattice basis splits off the free factor:

$$
\boxed{\mathcal O_K^\times\cong\mu(K)\times\mathbb Z^{r_1+r_2-1}.}
$$

This derives both finiteness and the unit rank from the stated compactness assumption, rather than assuming either conclusion to prove compactness.

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For this non-Archimedean [local field](../../../arithmetic.md#local-field), the [Schwartz-Bruhat space](../../../fourier-analysis.md#schwartz-bruhat-space) $\mathcal S(F)$ consists of locally constant, compactly supported complex-valued functions. Choose a nontrivial continuous [additive character](../../../analysis.md#additive-character) $\psi:F\to\mathbb C^\times$ of modulus one and an additive [Haar measure](../../../measure-theory.md#haar-measure) $dx$. We use the plus-sign convention for the [Fourier transform over a local field](../../../analysis.md#fourier-transform-over-a-local-field):

$$
\widehat f(y)=\int_F f(x)\psi(xy)\,dx.
$$

Compact support makes the integral absolutely convergent. The [additive character](../../../analysis.md#additive-character) and the scale of the [Haar measure](../../../measure-theory.md#haar-measure) are part of the definition; without them there is no canonical numerical transform.

Let $q=|\mathcal O_F/\pi_F\mathcal O_F|$, and write $V=\operatorname{vol}(\mathcal O_F)$. Define the integer $c$ by the [annihilator of the valuation ring](../../../analysis.md#annihilator-of-the-valuation-ring) $\mathcal O_F^\perp=\pi_F^c\mathcal O_F$. Equivalently, $\psi$ is trivial on $\pi_F^c\mathcal O_F$ and not on $\pi_F^{c-1}\mathcal O_F$. Such a conductor exists: continuity puts the image of some additive ball inside an arc containing no nontrivial circle subgroup, so the character is trivial on that ball; nontriviality bounds the possible ball exponents below. Then $H_n=\pi_F^n\mathcal O_F$ has volume $Vq^{-n}$ and [character annihilator](../../../analysis.md#character-annihilator) $H_n^\perp=\pi_F^{c-n}\mathcal O_F$.

Translation gives

$$
\widehat{\mathbf1_{a+H_n}}(y)=\psi(ay)\int_{H_n}\psi(ty)\,dt.
$$

The integral is the volume if $y\in H_n^\perp$. Otherwise translate it by $t_0\in H_n$ with $\psi(t_0y)\ne1$; [Haar measure](../../../measure-theory.md#haar-measure) invariance multiplies the same integral by a nonidentity scalar, so it must vanish. Thus

$$
\boxed{\widehat{\mathbf1_{a+\pi_F^n\mathcal O_F}}(y)=Vq^{-n}\psi(ay)\mathbf1_{\pi_F^{c-n}\mathcal O_F}(y).}
$$

Every [Schwartz-Bruhat function](../../../fourier-analysis.md#schwartz-bruhat-function) is a finite linear combination of such coset indicators: compactness of its support supplies a common sufficiently small translation subgroup on which it is constant, and finitely many of its cosets cover the support. The transform of each indicator has compact support and is locally constant, since $\psi$ has open kernel. Consequently **$\widehat f\in\mathcal S(F)$ for every $f\in\mathcal S(F)$**.

Apply the transform again to an indicator. The same character-orthogonality calculation, together with $(H_n^\perp)^\perp=H_n$, gives

$$
\widehat{\widehat{\mathbf1_{a+H_n}}}(x)=Vq^{-n}\operatorname{vol}(H_n^\perp)\mathbf1_{H_n}(-x-a)=V^2q^{-c}\mathbf1_{a+H_n}(-x).
$$

Choose the [self-dual Haar measure](../../../analysis.md#self-dual-haar-measure), characterized here by $V=q^{c/2}$. By linearity the desired [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) is

$$
\boxed{\widehat{\widehat f}(x)=f(-x).}
$$

In particular, one may rescale any nontrivial [additive character](../../../analysis.md#additive-character) to make $c=0$, and then take $V=1$. For a concrete construction, start with $\psi_0(x)=\psi_{\mathbb Q_p}(\operatorname{Tr}_{F/\mathbb Q_p}x)$, where the standard rational [additive character](../../../analysis.md#additive-character) has kernel $\mathbb Z_p$. Its annihilator is the [inverse different](../../../arithmetic.md#inverse-different) $\mathfrak D_{F/\mathbb Q_p}^{-1}$. If that ideal is $\pi_F^{-d}\mathcal O_F$, the rescaled character $\psi(x)=\psi_0(\pi_F^{-d}x)$ has $\mathcal O_F^\perp=\mathcal O_F$. This supplies the stated normalization and also explains how the [different ideal](../../../arithmetic.md#different-ideal) enters local [Fourier analysis](../../../fourier-analysis.md).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
