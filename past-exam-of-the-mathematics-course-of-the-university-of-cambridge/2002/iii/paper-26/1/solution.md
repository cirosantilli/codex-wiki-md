<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $q=e^{2\pi i\tau}$ and $\sigma_j(n)=\sum_{d\mid n}d^j$. Separate the $m=0$ terms in the [lattice Eisenstein series](../../../../../lattice-eisenstein-sum.md). Differentiating the [cosecant partial-fraction identity](../../../../../cosecant-partial-fraction-identity.md) $2k-2$ times gives, for $\Im z>0$,

$$
\sum_{n\in\mathbb Z}(z+n)^{-2k}
=\frac{(2\pi i)^{2k}}{(2k-1)!}\sum_{r\geq1}r^{2k-1}e^{2\pi irz}.
$$

The initial identity is $\sum_n(z+n)^{-2}=\pi^2\csc^2(\pi z)=-4\pi^2\sum_{r\geq1}re^{2\pi irz}$; differentiation accounts for the factorial and the sign. Pair $m$ and $-m$ and collect the products $mr$. [Absolute convergence](../../../../../absolute-convergence.md) of the lattice sum for $k\geq2$, and local uniform convergence of the resulting [power series](../../../../../power-series.md), justify these operations. Thus the requested [Fourier expansions](../../../../../fourier-series-split.md) are

$$
\boxed{G_{2k}(\tau)=2\zeta(2k)+\frac{2(2\pi i)^{2k}}{(2k-1)!}\sum_{n\geq1}\sigma_{2k-1}(n)q^n,\qquad
E_{2k}(\tau)=1-\frac{4k}{B_{2k}}\sum_{n\geq1}\sigma_{2k-1}(n)q^n.}
$$

Here $E_{2k}=G_{2k}/(2\zeta(2k))$, and the [Bernoulli numbers](../../../../../bernoulli-number.md) have convention $B_2=1/6$. The second formula uses Euler's even-value identity for the [Riemann zeta function](../../../../../riemann-zeta-function.md), $2\zeta(2k)=(-1)^{k+1}B_{2k}(2\pi)^{2k}/(2k)!$. In particular $E_4=1+240\sum\sigma_3(n)q^n$ and $E_6=1-504\sum\sigma_5(n)q^n$.

We need the rational, rather than merely complex, version of the [polynomial ring of level-one modular forms](../../../../../polynomial-ring-of-level-one-modular-forms.md). Recall how the [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) supplies its proof. For a nonzero weight-$w$ [modular form](../../../../../modular-form.md), with $\rho=e^{2\pi i/3}$,

$$
v_\infty(f)+\tfrac12v_i(f)+\tfrac13v_\rho(f)+\sum_{z\ne i,\rho}v_z(f)=w/12.
$$

Integrate $f'/f$ around a truncated [standard fundamental domain of the modular group](../../../../../standard-fundamental-domain-of-the-modular-group.md), indenting around boundary zeros. The paired vertical sides cancel by translation; pair the two halves of the circular edge using $f(-1/\tau)=\tau^wf(\tau)$. The logarithmic derivative of $\tau^w$ supplies $w/12$, while the top edge supplies $v_\infty(f)$. The half-disc and third-disc at the two elliptic points account for the fractions $1/2,1/3$. The [argument principle](../../../../../argument-principle.md) then gives the formula. All orders in it are nonnegative for a holomorphic [modular form](../../../../../modular-form.md). It follows that negative weights have no forms, $M_0=\mathbb C$, and $M_2=0$: a weight-two form vanishes at $i$, contributing at least $1/2>2/12$.

Define $\Delta_0=(E_4^3-E_6^2)/1728$. It is a weight-twelve [cusp form](../../../../../cusp-form.md) and its expansion starts with $q$. The [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) forces its order at infinity to be exactly one and leaves no interior zeros. Thus division by $\Delta_0$ identifies $S_w$ with $M_{w-12}$. Every nonnegative even $w\ne2$ has a monomial $E_4^aE_6^b$ of weight $w$: solve $2a+3b=w/2$, taking $b=0$ when $w/2$ is even and $b=1$ when it is odd and at least three. Subtract the constant coefficient of a [modular form](../../../../../modular-form.md) times such a monomial and divide by $\Delta_0$. Induction on weight proves generation by $E_4,E_6$.

If the original [Fourier coefficients](../../../../../fourier-coefficient.md) are rational, every step preserves rationality: both generators and $\Delta_0$ have rational expansions, and formal division by $\Delta_0=q+O(q^2)$ does too. This proves the [rational structure of level-one modular forms](../../../../../rational-structure-of-level-one-modular-forms.md). Write $E_{2k}=\sum r_{a,b}E_4^aE_6^b$ with $r_{a,b}\in\mathbb Q$ and $4a+6b=2k$. Rescaling gives

$$
G_{2k}=\sum_{4a+6b=2k}r_{a,b}\frac{2\zeta(2k)}{(2\zeta(4))^a(2\zeta(6))^b}G_4^aG_6^b.
$$

The [Bernoulli number](../../../../../bernoulli-number.md) formula above makes each zeta ratio rational: its powers of $\pi$ cancel precisely because the weights agree. This proves the required rational coefficients for the unnormalized [lattice Eisenstein sums](../../../../../lattice-eisenstein-sum.md).

Finally $S_8=S_{10}=0$ because the quotient weights are negative, and $S_{14}=0$ because $M_2=0$. In each of these weights a form is determined by its constant coefficient. The indicated monomials have that coefficient equal to one, so

$$
\boxed{E_8=E_4^2,\qquad E_{10}=E_4E_6,\qquad E_{14}=E_4^2E_6.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
