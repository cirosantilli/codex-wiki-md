# Paper 137

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_137.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_137.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [Fourier transform](../../../analysis.md#fourier-transform) normalization $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-2\pi ix\xi}\,dx$. A precise version of the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) is that, for every [Schwartz function](../../../fourier-analysis.md#schwartz-function) $f\in\mathcal S(\mathbb R)$,

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{m\in\mathbb Z}\widehat f(m).}
$$

Both series have [absolute convergence](../../../real-analysis.md#absolute-convergence). Here being a [Schwartz function](../../../fourier-analysis.md#schwartz-function) means being smooth with $\sup_x|x^a f^{(b)}(x)|<\infty$ for all nonnegative integers $a,b$. This hypothesis makes the sums and the termwise operations below legitimate; the formula is not being asserted for arbitrary integrable [functions](../../../function.md).

Form the [periodization of a Schwartz function](../../../fourier-analysis.md#periodization-of-a-schwartz-function) $P_f(x)=\sum_n f(x+n)$. Every differentiated series has [uniform convergence](../../../real-analysis.md#uniform-convergence) on $[0,1]$, by rapid decay, so $P_f$ is a smooth [periodic function](../../../function.md#periodic-function) of period one. Its $m$th [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) is

$$
\int_0^1P_f(x)e^{-2\pi imx}\,dx
=\sum_n\int_n^{n+1}f(u)e^{-2\pi imu}\,du=\widehat f(m).
$$

The interchange follows from [absolute convergence](../../../real-analysis.md#absolute-convergence) uniformly on this interval. [Integration by parts](../../../calculus.md#integration-by-parts) shows that these [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) decrease faster than every inverse power of $|m|$. Thus the [Fourier series](../../../fourier-series.md) converges absolutely and uniformly to $P_f$; for example the standard convergence theorem for twice continuously differentiable [periodic functions](../../../function.md#periodic-function) applies. Evaluating at zero proves the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula).

For $t>0$, scaling the given Gaussian [Fourier transform](../../../analysis.md#fourier-transform) gives

$$
\widehat{e^{-\pi t x^2}}(\xi)=t^{-1/2}e^{-\pi\xi^2/t}.
$$

Applying the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) gives the real-parameter [Jacobi theta function](../../../modular-function.md#jacobi-theta-function) transformation

$$
\boxed{\theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}=t^{-1/2}\theta(1/t).}
$$

For $\operatorname{Re}s>1$, termwise application of the [Mellin transform](../../../analysis.md#mellin-transform) is justified by integrating absolute values and gives

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\theta(t)-1)t^{s/2-1}\,dt.
$$

Each positive $n$ contributes $\Gamma(s/2)(\pi n^2)^{-s/2}$, and the factor one half removes the equal positive and negative terms. This is the [Mellin representation of the completed Riemann zeta function](../../../analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function).

Split the integral at one. On $(0,1)$, the [Jacobi theta function](../../../modular-function.md#jacobi-theta-function) transformation writes $\theta(t)-1=t^{-1/2}-1+t^{-1/2}(\theta(1/t)-1)$. Integrating the first two terms and substituting $u=1/t$ in the third yields the [pole-subtracted theta integral for the completed zeta function](../../../analytic-number-theory.md#pole-subtracted-theta-integral-for-the-completed-zeta-function):

$$
\Lambda(s)=\frac1{s-1}-\frac1s+
\frac12\int_1^\infty(\theta(t)-1)
\left(t^{s/2-1}+t^{(1-s)/2-1}\right)\,dt.
$$

The remaining integral is an [entire function](../../../complex-analysis.md#entire-function) of $s$: $\theta(t)-1=O(e^{-\pi t})$, and on each compact set of $s$ this exponential dominates all powers of $t$ and all factors arising from differentiation. It therefore supplies a [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) of $\Lambda$ to the whole plane, with simple [poles](../../../isolated-singularity.md#pole) at one and zero, of residues $1$ and $-1$, respectively. Its expression is unchanged by $s\mapsto1-s$.

The reciprocal [Gamma function](../../../complex-analysis.md#gamma-function) is entire, with simple zeros at its nonpositive integer arguments. Consequently

$$
\zeta(s)=\pi^{s/2}\Gamma(s/2)^{-1}\Lambda(s)
$$

is holomorphic everywhere except for a simple [pole](../../../isolated-singularity.md#pole) at $s=1$, of residue one. The apparent [pole](../../../isolated-singularity.md#pole) at $s=0$ cancels; in fact $\Gamma(s/2)^{-1}\sim s/2$ gives $\zeta(0)=-1/2$. This proves the [analytic continuation](../../../complex-analysis.md#analytic-continuation) of the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function). The completed [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) is

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

These are equalities of [meromorphic functions](../../../isolated-singularity.md#meromorphic-function); at apparent singularities they are interpreted by continuation. Equivalently, $\xi(s)=\tfrac12s(s-1)\Lambda(s)$ is an [entire function](../../../complex-analysis.md#entire-function) with $\xi(s)=\xi(1-s)$.

## 2

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Extend the [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) $\chi$ periodically to all [integers](../../../number-theory.md#integer), putting $\chi(n)=0$ when $(n,N)>1$. Its [Dirichlet L-function](../../../algebraic-number-theory.md#dirichlet-l-function), initially on $\operatorname{Re}s>1$, is

$$
\boxed{L(\chi,s)=\sum_{n\geq1}\chi(n)n^{-s}
=\prod_{p\nmid N}(1-\chi(p)p^{-s})^{-1}.}
$$

The [Euler product](../../../analytic-number-theory.md#euler-product) follows from unique [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) and [absolute convergence](../../../real-analysis.md#absolute-convergence); a [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) is completely multiplicative on this extension. Write $\chi_0$ for the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character), equal to one on units and zero elsewhere.

For a [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) $\chi$, [character orthogonality](../../../representation-theory.md#character-orthogonality) gives $\sum_{a=1}^N\chi(a)=0$. Explicitly, multiplication by a unit $u$ with $\chi(u)\ne1$ permutes the unit residues and multiplies this sum by $\chi(u)$, forcing it to vanish. For $t>0$ set

$$
H_\chi(t)=\sum_{n\geq1}\chi(n)e^{-nt}
=\frac{\sum_{a=1}^N\chi(a)e^{-at}}{1-e^{-Nt}}.
$$

The numerator is $O(t)$ at zero and the denominator is $Nt+O(t^2)$, so $H_\chi$ is bounded, indeed analytic, near zero; it decays exponentially at infinity. Initially for $\operatorname{Re}s>1$, [absolute convergence](../../../real-analysis.md#absolute-convergence) justifies

$$
\Gamma(s)L(\chi,s)=\int_0^\infty H_\chi(t)t^{s-1}\,dt.
$$

This [Mellin transform](../../../analysis.md#mellin-transform) integral is holomorphic for $\operatorname{Re}s>0$, locally uniformly in $s$, and division by the [Gamma function](../../../complex-analysis.md#gamma-function) proves the requested [analytic continuation](../../../complex-analysis.md#analytic-continuation) to the left of the line one.

In fact, the same argument proves [Mellin continuation of a nonprincipal Dirichlet L-function](../../../algebraic-number-theory.md#mellin-continuation-of-a-nonprincipal-dirichlet-l-function) to the entire plane. If $H_\chi(t)=\sum_{r=0}^M c_rt^r+O(t^{M+1})$ at zero, subtract this [Taylor polynomial](../../../calculus.md#taylor-polynomial) on $(0,1)$ and add its explicit integrals:

$$
\Gamma(s)L(\chi,s)=\int_1^\infty H_\chi(t)t^{s-1}\,dt
+\sum_{r=0}^M\frac{c_r}{s+r}
+\int_0^1\left(H_\chi(t)-\sum_{r=0}^M c_rt^r\right)t^{s-1}\,dt.
$$

The last integral is holomorphic on $\operatorname{Re}s>-M-1$. Its possible simple [poles](../../../isolated-singularity.md#pole) at nonpositive integers cancel against zeros of $1/\Gamma(s)$. Letting $M$ increase shows that $L(\chi,s)$ is an [entire function](../../../complex-analysis.md#entire-function), without any primitivity assumption.

For real $s>1$, use the absolutely convergent [Euler product](../../../analytic-number-theory.md#euler-product) logarithm

$$
B_\chi(s)=\sum_{p\nmid N}\sum_{m\geq1}\frac{\chi(p)^m}{mp^{ms}}
=F_\chi(s)+R_\chi(s),\qquad e^{B_\chi(s)}=L(\chi,s).
$$

The higher-power remainder has the uniform estimate

$$
|R_\chi(s)|\leq\sum_p\sum_{m\geq2}p^{-m}
=\sum_p\frac1{p(p-1)}\leq\sum_{n\geq2}\frac1{n(n-1)}=1.
$$

For a [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) $\chi$, invoke the allowed [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../analytic-number-theory.md#nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one). Its holomorphy and nonvanishing give a [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) on a small disk about one. On the connected real interval $1<s<1+\eta$, $B_\chi(s)$ differs from this logarithm by a fixed element of $2\pi i\mathbb Z$: the difference is continuous with exponential one. Thus the [prime-character sum near one](../../../analytic-number-theory.md#prime-character-sum-near-one) is bounded. This branch argument is needed for complex-valued [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character).

For $\chi_0$,

$$
L(\chi_0,s)=\zeta(s)\prod_{p\mid N}(1-p^{-s}).
$$

The finite product has a positive limit as $s\downarrow1$, and the residue-one [pole](../../../isolated-singularity.md#pole) of the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) gives

$$
\boxed{F_{\chi_0}(s)=\log\frac1{s-1}+O(1)\longrightarrow+\infty,
\qquad F_\chi(s)=O(1)\quad(\chi\ne\chi_0).}
$$

Here $O(1)$ for nonprincipal [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character) means bounded complex magnitude.

Finally, for a [residue class](../../../number-theory.md#residue-class) $a$ coprime to $N$, [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) gives

$$
\sum_{p\equiv a\pmod N}p^{-s}
=\frac1{\varphi(N)}\sum_{\chi\bmod N}\overline{\chi(a)}F_\chi(s)
=\frac1{\varphi(N)}\log\frac1{s-1}+O(1).
$$

Only [primes](../../../number-theory.md#prime-number) not dividing $N$ occur, so the character orthogonality applies to every term. This sum diverges as $s\downarrow1$. A finite collection of [primes](../../../number-theory.md#prime-number) would give a bounded sum, a contradiction. **Every reduced residue class contains infinitely many [primes](../../../number-theory.md#prime-number).** This is the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions); the coprimality hypothesis is essential.

## 3

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group): for a nonzero [modular form](../../../modular-function.md#modular-form) of weight $k$ on $SL_2(\mathbb Z)$,

$$
v_\infty(f)+\frac12v_i(f)+\frac13v_\rho(f)
+\sum_{z\ne i,\rho}v_z(f)=\frac{k}{12},\qquad\rho=e^{2\pi i/3}.
$$

The sum contains one representative of each other [modular group](../../../modular-function.md#modular-group) orbit of zeros. The orders are nonnegative because $f$ is holomorphic on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) and at infinity. The half and third weights account for the [elliptic stabilizers of the modular group](../../../modular-function.md#elliptic-stabilizers-of-the-modular-group).

In weight two, the transformation under $S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ at its fixed point gives $f(i)=i^2f(i)=-f(i)$. Thus any nonzero $f$ would have $v_i(f)\geq1$. The [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group) would give a left side at least $1/2$ and a right side $1/6$, which is impossible. Therefore the unheaded request is answered by [vanishing of weight-two level-one modular forms](../../../modular-function.md#vanishing-of-weight-two-level-one-modular-forms):

$$
\boxed{M_2(\Gamma(1))=\{0\}.}
$$

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The displayed definition uses [iterated Eisenstein summation in weight two](../../../modular-function.md#iterated-eisenstein-summation-in-weight-two): the sum in $n$ is evaluated before the sum in $m$, with the single $(0,0)$ term omitted. This order is essential. The two-dimensional lattice series does not have [absolute convergence](../../../real-analysis.md#absolute-convergence), so arbitrary rearrangement would not be justified.

For noninteger $w$, the [cosecant partial-fraction identity](../../../fourier-series.md#cosecant-partial-fraction-identity) is

$$
\sum_{n\in\mathbb Z}\frac1{(w+n)^2}=\pi^2\csc^2(\pi w).
$$

For completeness, apply the [residue theorem](../../../analysis.md#residue-theorem) to $\pi\cot(\pi\zeta)/(\zeta-w)^2$ on squares with large half-integer sides. The [cotangent](../../../geometry-and-topology.md#cotangent) is bounded on the contours and the integral is $O(R^{-1})$. Its residues at the integers are $(n-w)^{-2}$ and its residue at $w$ is $-\pi^2\csc^2(\pi w)$, proving the formula. If $\operatorname{Im}w>0$, the geometric-series expression $\cot(\pi w)=-i(1+2\sum_{r\geq1}e^{2\pi irw})$, differentiated termwise, gives the [cotangent partial-fraction Fourier kernel](../../../fourier-series.md#cotangent-partial-fraction-fourier-kernel)

$$
\pi^2\csc^2(\pi w)=-4\pi^2\sum_{r\geq1}r e^{2\pi irw}.
$$

Put $q=e^{2\pi iz}$ with $z$ in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). For positive $m$, this gives $-4\pi^2\sum_{r\geq1}r q^{mr}$. Negative $m$ gives the same value, by replacing $n$ with $-n$ in its inner sum. The $m=0$ row is $\sum_{n\ne0}n^{-2}=\pi^2/3$, by the [Basel problem](../../../analytic-number-theory.md#basel-problem). The resulting series in $m,r$ does have [absolute convergence](../../../real-analysis.md#absolute-convergence), locally uniformly in $z$, so collecting the coefficient at $q^\ell$ is legitimate:

$$
G_2(z)=\frac{\pi^2}{3}-8\pi^2\sum_{m,r\geq1}r q^{mr}
=\frac{\pi^2}{3}-8\pi^2\sum_{\ell\geq1}\sigma_1(\ell)q^\ell.
$$

The coefficient is the [sum-of-divisors function](../../../number-theory.md#sum-of-divisors-function), since $r$ runs over the positive divisors of $\ell$. Thus

$$
\boxed{G_2(z)=\frac{\pi^2}{3}E_2(z).}
$$

There is no conflict with [vanishing of weight-two level-one modular forms](../../../modular-function.md#vanishing-of-weight-two-level-one-modular-forms): the [Eisenstein series of weight two](../../../modular-function.md#eisenstein-series-of-weight-two) has an anomalous transformation term, so it is not a weight-two [modular form](../../../modular-function.md#modular-form).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $D=(2\pi i)^{-1}d/dz=q\,d/dq$ and use the [Serre derivative](../../../modular-function.md#serre-derivative) $D_kf=Df-(k/12)E_2f$. Translation invariance of $f$ and the [Eisenstein series of weight two](../../../modular-function.md#eisenstein-series-of-weight-two) gives $D_kf(z+1)=D_kf(z)$.

Differentiate the weight-$k$ transformation $f(-1/z)=z^kf(z)$. The [chain rule](../../../calculus.md#chain-rule) yields

$$
Df(-1/z)=z^{k+2}Df(z)+\frac{k}{2\pi i}z^{k+1}f(z).
$$

The assumed transformation of the [Eisenstein series of weight two](../../../modular-function.md#eisenstein-series-of-weight-two) gives

$$
\frac{k}{12}E_2(-1/z)f(-1/z)
=\frac{k}{12}z^{k+2}E_2(z)f(z)+\frac{k}{2\pi i}z^{k+1}f(z).
$$

Subtracting cancels the extra term. Hence $D_kf(-1/z)=z^{k+2}D_kf(z)$. Since $S$ and $T=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ generate the [modular group](../../../modular-function.md#modular-group), these two transformations prove the weight-$k+2$ law for all its elements. Holomorphy on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) follows from the formula.

For the [Fourier expansion of a modular form](../../../modular-function.md#fourier-expansion-of-a-modular-form) $f=\sum_{n\geq0}a_nq^n$, differentiation gives $Df=\sum_{n\geq1}na_nq^n$. The product of the convergent series for $E_2$ and $f$ likewise has no negative powers. Thus $D_kf$ is [holomorphic at a cusp](../../../modular-function.md#holomorphic-at-a-cusp) at infinity, and therefore at every cusp of the [modular group](../../../modular-function.md#modular-group). Its constant coefficient is $-ka_0/12$. Since $k>0$, it vanishes exactly when $a_0=0$. Consequently

$$
\boxed{D_kf\in M_{k+2}(\Gamma(1)),\qquad
D_kf\in S_{k+2}(\Gamma(1))\iff f\in S_k(\Gamma(1)).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Apply the [Serre derivative](../../../modular-function.md#serre-derivative) in weight twelve to the [modular discriminant](../../../modular-function.md#modular-discriminant). The preceding result makes $D_{12}\Delta=D\Delta-E_2\Delta$ a weight-fourteen [cusp form](../../../modular-function.md#cusp-form). The [vanishing of weight-fourteen level-one cusp forms](../../../modular-function.md#vanishing-of-weight-fourteen-level-one-cusp-forms) follows directly from the [valence formula for the modular group](../../../modular-function.md#valence-formula-for-the-modular-group): a nonzero such form has order at infinity at least one, and $f(i)=i^{14}f(i)=-f(i)$ forces order at $i$ at least one. Thus its weighted number of zeros would be at least $1+1/2>14/12$, a contradiction. Therefore $D\Delta=E_2\Delta$.

Compare the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) at positive indices using $\Delta=\sum_{n\geq1}\tau(n)q^n$ and $E_2=1-24\sum_{r\geq1}\sigma_1(r)q^r$. This gives $n\tau(n)=\tau(n)-24\sum_{r=1}^{n-1}\sigma_1(r)\tau(n-r)$. For the [Ramanujan tau function](../../../modular-function.md#ramanujan-tau-function), the concise recurrence is

$$
\boxed{(1-n)\tau(n)=24\sum_{r=1}^{n-1}\sigma_1(r)\tau(n-r)\qquad(n\geq1).}
$$

At $n=1$ the sum is empty and both sides are zero; normalization supplies $\tau(1)=1$. For instance the next coefficient is $\tau(2)=-24$.

## 4

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

First establish [rational conjugation of finite-index modular subgroups](../../../modular-function.md#rational-conjugation-of-finite-index-modular-subgroups) without assuming that $\Gamma$ is a [congruence subgroup](../../../group-theory.md#congruence-subgroup). Multiply $\gamma$ by a positive integer to obtain an integral [matrix](../../../vector-space.md#matrix) $A$, and let $D=\det A>0$. Conjugation is unchanged by this scalar. If $h=I+DB\in\Gamma(D)$, then

$$
AhA^{-1}=I+AB\operatorname{adj}(A)\in SL_2(\mathbb Z).
$$

Thus the [principal congruence subgroup](../../../group-theory.md#principal-congruence-subgroup) $\Gamma(D)$ is contained in $H=SL_2(\mathbb Z)\cap\gamma^{-1}SL_2(\mathbb Z)\gamma$. It has finite index because reduction modulo $D$ has finite image. Inside $H$, pullback under conjugation of $\Gamma$ has relative index at most $[SL_2(\mathbb Z):\Gamma]$. Consequently

$$
\boxed{[SL_2(\mathbb Z):\Gamma']<\infty,
\quad\Gamma'=SL_2(\mathbb Z)\cap\gamma^{-1}\Gamma\gamma.}
$$

This argument does not assert that an arbitrary [finite-index subgroup](../../../group.md#finite-index-subgroup) contains a [principal congruence subgroup](../../../group-theory.md#principal-congruence-subgroup).

Use the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator)

$$
(f|_k\gamma)(z)=(\det\gamma)^{k/2}(cz+d)^{-k}f\left(\frac{az+b}{cz+d}\right),
\quad\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix},\quad\det\gamma>0.
$$

The positive real power of the [determinant](../../../linear-algebra.md#determinant) is used; on $SL_2(\mathbb Z)$ this reduces to the usual [slash operator for modular forms](../../../modular-function.md#slash-operator-for-modular-forms). The [automorphy factor](../../../modular-function.md#automorphy-factor) identity gives the right-action rule $(f|_k\gamma)|_k\eta=f|_k(\gamma\eta)$.

A [modular form on a finite-index subgroup](../../../modular-function.md#modular-form-on-a-finite-index-subgroup) of integer weight $k$ is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), invariant under this weight-$k$ action of $\Gamma$, and [holomorphic at a cusp](../../../modular-function.md#holomorphic-at-a-cusp) at each of its cusps. A [cusp of a modular group](../../../modular-function.md#cusp-of-a-modular-group) is a $\Gamma$ orbit in $\mathbb P^1(\mathbb Q)$. If $\sigma\in SL_2(\mathbb Z)$ carries infinity to its representative, choose a positive integer $h$ with $\sigma T^h\sigma^{-1}\in\Gamma$. Such $h$ exists by finite index. Then $f|_k\sigma$ is periodic and has a convergent expansion in $q_h=e^{2\pi iz/h}$ near zero; holomorphy means no negative exponents, and being a [cusp form](../../../modular-function.md#cusp-form) means zero constant term. Using an actual translation period avoids possible signs if a smaller [width of a cusp](../../../modular-function.md#width-of-a-cusp) is defined only modulo the center, particularly in odd weights.

For [cusp holomorphy under rational slash operators](../../../modular-function.md#cusp-holomorphy-under-rational-slash-operators), choose $\sigma\in SL_2(\mathbb Z)$ with $\sigma\infty=\gamma\infty$, possible by completing a primitive integer pair to a determinant-one [matrix](../../../vector-space.md#matrix). Then $\sigma^{-1}\gamma=\begin{pmatrix}a&b\\0&d\end{pmatrix}$, with $a/d>0$. Up to a nonzero constant factor,

$$
f|_k\gamma(z)=(f|_k\sigma)((a/d)z+b/d).
$$

The imaginary part of the argument tends to infinity with that of $z$, so this remains bounded by the cusp expansion of $f|_k\sigma$. It tends to zero if $f$ is a [cusp form](../../../modular-function.md#cusp-form). Moreover $f|_k\gamma$ is invariant under $\Gamma'$: for $\eta\in\Gamma'$, $\gamma\eta\gamma^{-1}\in\Gamma$ and the right-action rule applies. Finite index gives a translation period for $\Gamma'$, so boundedness is a [removable singularity](../../../isolated-singularity.md#removable-singularity) at zero in that periodic parameter. This proves holomorphy at infinity. For every other cusp, apply the same argument to the rational [matrix](../../../vector-space.md#matrix) $\gamma\rho$, with $\rho\in SL_2(\mathbb Z)$. Thus all cusp conditions hold, and

$$
\boxed{f|_k\gamma\in M_k(\Gamma').}
$$

For the [character twist by rational translations of a cusp form](../../../modular-function.md#character-twist-by-rational-translations-of-a-cusp-form), put $B_j=\begin{pmatrix}1&j/N\\0&1\end{pmatrix}$ and $K=\Gamma_1(N)\cap\Gamma_0(N^2)$. For $\eta=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in K$, direct conjugation gives

$$
B_j\eta B_j^{-1}=\begin{pmatrix}
a+jc/N&b+j(d-a)/N-j^2c/N^2\\
c&d-jc/N
\end{pmatrix}\in SL_2(\mathbb Z).
$$

Indeed $N^2\mid c$ and $a\equiv d\equiv1\pmod N$. Every $f|_kB_j=f(z+j/N)$ is therefore $K$-invariant and vanishes at all its cusps by the preceding rational-translate argument. Their finite weighted sum is a [cusp form](../../../modular-function.md#cusp-form), for every [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character):

$$
\boxed{f_\chi\in S_k(\Gamma_1(N)\cap\Gamma_0(N^2)).}
$$

There is, however, **a missing primitivity hypothesis in the printed final expansion claim**. The exact [Fourier expansion of a modular form](../../../modular-function.md#fourier-expansion-of-a-modular-form) is always

$$
\boxed{f_\chi(z)=\sum_{n\geq1}a_n(f)S_{\overline\chi}(n)q^n,
\quad S_{\overline\chi}(n)=\sum_{j\in(\mathbb Z/N\mathbb Z)^\times}\overline{\chi(j)}e^{2\pi inj/N}.}
$$

Values of a [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) on units have modulus one, so $\chi(j)^{-1}=\overline{\chi(j)}$. For unit $n$, substitution gives $S_{\overline\chi}(n)=\chi(n)g(\overline\chi)$, where $g$ is the [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character). For nonunit $n$, this vanishing formula requires a [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character).

Here is its proof in that case. Choose a [prime](../../../number-theory.md#prime-number) $p\mid(n,N)$. Primitivity supplies a unit $u\equiv1\pmod{N/p}$ with $\chi(u)\ne1$: otherwise the character would factor through the surjective reduction to units modulo $N/p$. Surjectivity follows by lifting a unit and, if needed, adjusting the lift to avoid the additional prime $p$, using the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem). Multiplication by $u$ fixes $e^{2\pi inj/N}$ because $p\mid n$, but multiplies the character factor by a nontrivial constant. Hence $S_{\overline\chi}(n)=0$. The [finite Fourier transform of a primitive Dirichlet character](../../../algebraic-number-theory.md#finite-fourier-transform-of-a-primitive-dirichlet-character) now gives the corrected formula

$$
\boxed{f_\chi=g(\overline\chi)\sum_{n\geq1}\chi(n)a_n(f)q^n
\quad\text{if }\chi\text{ is primitive modulo }N.}
$$

The constant is nonzero: finite exponential orthogonality gives $\sum_{n\bmod N}|S_{\overline\chi}(n)|^2=N\varphi(N)$, whereas the proved formula makes this $\varphi(N)|g(\overline\chi)|^2$. Thus $|g(\overline\chi)|=\sqrt N$.

For a concrete counterexample to the printed unrestricted claim, take $N=2$, the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character), and $f=\Delta$. The translation sum is $\Delta(z+1/2)=\sum_n(-1)^n\tau(n)q^n$, whose $q^2$ coefficient is $-24$. Any constant multiple of the proposed odd-index-only series has $q^2$ coefficient zero. Thus the general modularity conclusion is proved, while the claimed simplification is false without the stated extra hypothesis.

## 5

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a weight-$k$ [cusp form](../../../modular-function.md#cusp-form), the [invariant norm of a modular form](../../../modular-function.md#invariant-norm-of-a-modular-form) $y^{k/2}|f(z)|$, with $y=\operatorname{Im}z$, is unchanged by the [modular group](../../../modular-function.md#modular-group): $\operatorname{Im}(\gamma z)=y/|cz+d|^2$ and $|f(\gamma z)|=|cz+d|^k|f(z)|$ cancel exactly.

Every orbit meets the [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) $\mathcal F=\{z:|\operatorname{Re}z|\leq1/2,\ |z|\geq1\}$, where $y\geq\sqrt3/2$. The [Fourier expansion of a modular form](../../../modular-function.md#fourier-expansion-of-a-modular-form) at the cusp has $f(q)=q h(q)$, with $h$ holomorphic near zero, since $f$ is a [cusp form](../../../modular-function.md#cusp-form). Thus $|f(x+iy)|=O(e^{-2\pi y})$ uniformly in $x$ as $y\to\infty$, and $y^{k/2}|f|$ tends to zero there. On the remaining compact part of $\mathcal F$ it is bounded by continuity. Invariance therefore gives

$$
\boxed{B:=\sup_{z\in\mathfrak H}y^{k/2}|f(z)|<\infty.}
$$

For every $y>0$, [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) extraction gives

$$
a_n(f)=e^{2\pi ny}\int_0^1f(x+iy)e^{-2\pi inx}\,dx,
\qquad |a_n(f)|\leq B e^{2\pi ny}y^{-k/2}.
$$

For $n\geq1$, minimize the last factor by taking $y=k/(4\pi n)$. This proves the [Fourier coefficient bound for a cusp form](../../../modular-function.md#fourier-coefficient-bound-for-a-cusp-form)

$$
\boxed{|a_n(f)|\leq B\left(\frac{4\pi e}{k}\right)^{k/2}n^{k/2}<Cn^{k/2},
\quad C=B\left(\frac{4\pi e}{k}\right)^{k/2}+1.}
$$

The assertion concerns positive indices; the constant coefficient vanishes because $f$ is a [cusp form](../../../modular-function.md#cusp-form).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Write $\Gamma=SL_2(\mathbb Z)$ and $G=GL_2(\mathbb Q)^+$. The [double-coset Hecke algebra](../../../group-theory.md#double-coset-hecke-algebra) consists of $\Gamma$-bi-invariant complex [functions](../../../function.md) on $G$ supported on finitely many [double cosets](../../../group-theory.md#double-coset), with convolution

$$
(h_1*h_2)(g)=\sum_{\Gamma x\in\Gamma\backslash G}h_1(gx^{-1})h_2(x).
$$

Each [double coset](../../../group-theory.md#double-coset) has finitely many orbits under left multiplication by $\Gamma$, by [rational conjugation of finite-index modular subgroups](../../../modular-function.md#rational-conjugation-of-finite-index-modular-subgroups). Thus the sum is finite and independent of representatives. The characteristic functions of the [double cosets](../../../group-theory.md#double-coset) form its basis, and its right action on invariant [modular forms](../../../modular-function.md#modular-form) is $f*h=\sum_{\Gamma x}h(x)f|_kx$, using the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator).

For a positive integer $n$, let $\mathcal M_n$ be all integral two-by-two [matrices](../../../vector-space.md#matrix) of positive [determinant](../../../linear-algebra.md#determinant) $n$. It is $\Gamma$-bi-invariant. Define $T(n)$ to be its [indicator function](../../../measure-theory.md#indicator-function), equivalently the sum of the distinct [double cosets](../../../group-theory.md#double-coset) it contains, each with coefficient one. This is the convention consistent with the requested formula. For composite $n$, it need not be the single [double coset](../../../group-theory.md#double-coset) of $\operatorname{diag}(1,n)$: for instance $2I\in\mathcal M_4$ cannot lie in that [double coset](../../../group-theory.md#double-coset), since multiplying by unimodular integral [matrices](../../../vector-space.md#matrix) preserves the greatest common divisor of the entries.

Prove all the needed subgroup facts directly. For a [finite-index subgroup](../../../group.md#finite-index-subgroup) $L\subseteq\mathbb Z^2$, take $a$ to be the least positive first coordinate appearing in $L$ and $d$ the least positive second coordinate on its intersection with the second axis. Euclidean division then shows that the first-coordinate projection is $a\mathbb Z$ and $L\cap(\{0\}\times\mathbb Z)=\{0\}\times d\mathbb Z$. Positivity follows, for example, because the finite [quotient group](../../../group-theory.md#quotient-group) kills a nonzero multiple of each coordinate vector. Choose $(a,b)\in L$ and reduce $b$ modulo $d$ to $0\leq b<d$. Every vector of $L$ has first coordinate a multiple of $a$, and subtracting that multiple of $(a,b)$ leaves a multiple of $(0,d)$. Therefore these two vectors form a [basis](../../../vector-space.md#basis) of $L$. The parameters $a,d,b$ are unique. Reducing the first coordinate modulo $a$ and then the second modulo $d$ gives precisely $ad$ quotient representatives, so $[\mathbb Z^2:L]=ad$.

Apply this [row Hermite normal form in rank two](../../../vector-space.md#row-hermite-normal-form-in-rank-two) to the [row lattice](../../../vector-space.md#row-lattice-of-an-integer-matrix) of an integral [matrix](../../../vector-space.md#matrix) $A$ with $\det A=n$. Its [row lattice](../../../vector-space.md#row-lattice-of-an-integer-matrix) contains $n\mathbb Z^2$, since $\operatorname{adj}(A)A=nI$, so it has finite index. Its two rows and the displayed two rows are [bases](../../../vector-space.md#basis) of the same [row lattice](../../../vector-space.md#row-lattice-of-an-integer-matrix). The two inverse change-of-basis [matrices](../../../vector-space.md#matrix) have integer entries, so their [determinants](../../../linear-algebra.md#determinant) are integers whose product is one. Thus the change-of-basis [matrix](../../../vector-space.md#matrix) has [determinant](../../../linear-algebra.md#determinant) $\pm1$; since both orientations are positive, its [determinant](../../../linear-algebra.md#determinant) is one. Thus each orbit under left multiplication by $\Gamma$ has exactly one of the [determinant-n matrix representatives for Hecke operators](../../../modular-function.md#determinant-n-matrix-representatives-for-hecke-operators)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d>0,\quad ad=n,\quad0\leq b<d.
$$

There are $\sum_{d\mid n}d$ such representatives, proving finiteness as well as the formula. The subgroup argument is a proof of the relevant [Hermite normal form](../../../vector-space.md#hermite-normal-form), not an invocation of an unproved lattice classification.

Consequently the normalized [Hecke operator](../../../modular-function.md#hecke-operator) is

$$
\boxed{T_nf=n^{k/2-1}\sum_{ad=n}\sum_{b=0}^{d-1}
 f|_k\begin{pmatrix}a&b\\0&d\end{pmatrix}.}
$$

It preserves $M_k(\Gamma)$: right multiplication by $\Gamma$ permutes the left-multiplication orbits in $\mathcal M_n$, giving invariance, and [cusp holomorphy under rational slash operators](../../../modular-function.md#cusp-holomorphy-under-rational-slash-operators) gives the holomorphy of each term at every cusp.

For a triangular representative the [determinant-normalized slash operator](../../../modular-function.md#determinant-normalized-slash-operator) is $f|_kA=n^{k/2}d^{-k}f((az+b)/d)$. Summing the [Fourier expansion of a modular form](../../../modular-function.md#fourier-expansion-of-a-modular-form) over $b$ kills every index not divisible by $d$, by finite exponential orthogonality. Thus

$$
T_nf=n^{k-1}\sum_{ad=n}d^{1-k}\sum_{\ell\geq0}a_{d\ell}(f)q^{a\ell}.
$$

The [Fourier coefficients of a composite-index Hecke operator](../../../modular-function.md#fourier-coefficients-of-a-composite-index-hecke-operator) are therefore

$$
\boxed{a_r(T_nf)=\sum_{a\mid\gcd(n,r)}a^{k-1}a_{nr/a^2}(f)\quad(r\geq1),
\qquad a_0(T_nf)=\sigma_{k-1}(n)a_0(f).}
$$

In particular $a_1(T_nf)=a_n(f)$. If $T_nf=\lambda f$, comparison of the $q$ coefficients gives

$$
\boxed{a_n(f)=\lambda a_1(f).}
$$

Finally suppose $a_0(f)\ne0$ and $f$ is a simultaneous eigenfunction. Constant coefficients force $\lambda_n=\sigma_{k-1}(n)$, so $a_n(f)=a_1(f)\sigma_{k-1}(n)$ for all $n\geq1$. Weight two cannot occur, by [vanishing of weight-two level-one modular forms](../../../modular-function.md#vanishing-of-weight-two-level-one-modular-forms). For even $k\geq4$, use the normalized [Eisenstein series](../../../modular-function.md#eisenstein-series) with its [Fourier expansion of a normalized Eisenstein series](../../../modular-function.md#fourier-expansion-of-a-normalized-eisenstein-series)

$$
E_k=1+c_k\sum_{n\geq1}\sigma_{k-1}(n)q^n,
\qquad c_k=-\frac{2k}{B_k}\ne0,
$$

where $B_k$ is the [Bernoulli number](../../../number-theory.md#bernoulli-number). Then $h=f-a_0(f)E_k$ is a [cusp form](../../../modular-function.md#cusp-form) with coefficients $(a_1(f)-a_0(f)c_k)\sigma_{k-1}(n)$. The [Fourier coefficient bound for a cusp form](../../../modular-function.md#fourier-coefficient-bound-for-a-cusp-form) bounds these by $O(n^{k/2})$, but at arbitrarily large [primes](../../../number-theory.md#prime-number) $p$ their magnitude is $|a_1-a_0c_k|(1+p^{k-1})$. Since $k-1>k/2$, the coefficient factor must vanish. All coefficients of $h$ then vanish, including its constant coefficient, so $h=0$ by its cusp expansion and the [identity theorem](../../../complex-analysis.md#identity-theorem). This proves the [noncuspidal level-one Hecke eigenform](../../../modular-function.md#noncuspidal-level-one-hecke-eigenform) characterization:

$$
\boxed{f=a_0(f)E_k\qquad(k\geq4).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
