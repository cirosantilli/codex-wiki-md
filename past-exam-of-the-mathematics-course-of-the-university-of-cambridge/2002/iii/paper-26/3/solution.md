<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Extend $\chi$ by zero to integers not coprime to $N$, and write $g(\chi)=\sum_{a\bmod N}\chi(a)e^{2\pi ia/N}$ for its [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md). We use the analytic branch of $\sqrt{-i\tau}$ that is positive when $\tau$ is positive imaginary. With the convention $\widehat F(t)=\int_{\mathbb R}F(x)e^{-2\pi ixt}\,dx$, the [Gaussian Fourier transform](../../../../../fourier-transform-of-a-gaussian.md) and its differentiated version are

$$
\widehat{e^{\pi i\tau x^2}}(t)=(-i\tau)^{-1/2}e^{-\pi it^2/\tau},\qquad
\widehat{x e^{\pi i\tau x^2}}(t)=\frac{t}{\tau}(-i\tau)^{-1/2}e^{-\pi it^2/\tau}.
$$

The first formula follows by completing the square, first on the imaginary axis and then by [analytic continuation](../../../../../analytic-continuation.md); the second follows by differentiating the [Fourier transform](../../../../../fourier-transform.md) in $t$. All the functions are [Schwartz functions](../../../../../schwartz-function.md) on the real axis.

For completeness, the [finite Fourier transform of a primitive Dirichlet character](../../../../../finite-fourier-transform-of-a-primitive-dirichlet-character.md) satisfies

$$
\sum_{a\bmod N}\chi(a)e^{2\pi ira/N}=g(\chi)\overline\chi(r).
$$

For a unit $r$ this is substitution by its inverse. If $p\mid(r,N)$, primitivity supplies a unit $u\equiv1\pmod{N/p}$ with $\chi(u)\ne1$: otherwise the character would factor through modulus $N/p$. Multiplication by $u$ fixes the additive exponential but multiplies the sum by $\chi(u)$, so the sum vanishes. This proves the identity also on nonunits. Finite [Parseval identity](../../../../../parseval-identity.md) now gives $|g(\chi)|^2=N$, since exactly $\varphi(N)$ frequencies have nonzero character values. In particular this [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md) is nonzero.

Apply [Poisson summation](../../../../../poisson-summation-formula.md) to each residue class: $\sum_jF(a+Nj)=N^{-1}\sum_r e^{2\pi ira/N}\widehat F(r/N)$. Multiply by $\chi(a)$ and sum over $a$. The formulas above give the two [character theta transformations](../../../../../character-theta-transformation.md)

$$
\boxed{\theta_\chi(\tau)=\frac{g(\chi)}{N\sqrt{-i\tau}}\,
\theta_{\overline\chi}\!\left(-\frac1{N^2\tau}\right)\quad\text{if }\chi(-1)=1,}
$$

and

$$
\boxed{\widetilde\theta_\chi(\tau)=\frac{g(\chi)}{iN^2(-i\tau)^{3/2}}\,
\widetilde\theta_{\overline\chi}\!\left(-\frac1{N^2\tau}\right)\quad\text{if }\chi(-1)=-1.}
$$

In the odd case the prefactor originally reads $g(\chi)/(N^2\tau\sqrt{-i\tau})$; using $\tau=i(-i\tau)$ explains the factor $i$. Opposite parity makes the corresponding series identically zero by pairing $n,-n$. This is why the weight-three-halves series is needed for odd [Dirichlet characters](../../../../../dirichlet-character.md).

To deduce the products from these transformations, use two specific [primitive Dirichlet characters](../../../../../primitive-dirichlet-character.md). The even character $\chi_{12}$ takes values $1,-1,-1,1$ on $1,5,7,11$ modulo twelve. It is primitive: its values do not factor through six or four, hence through no proper divisor of twelve. Its [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md) is $2\sqrt3=\sqrt{12}$. Put

$$
A(\tau)=\tfrac12\theta_{\chi_{12}}(\tau/12)=\tfrac12\sum_n\chi_{12}(n)q^{n^2/24}.
$$

The even transformation gives $A(-1/\tau)=\sqrt{-i\tau}\,A(\tau)$; also $A(\tau+1)=e^{\pi i/12}A(\tau)$, since each nonzero term has $n^2\equiv1\pmod{24}$. Thus $A^{24}$ transforms as a weight-twelve [modular form](../../../../../modular-form.md) under the generators $S,T$ of the [modular group](../../../../../modular-group.md). It is holomorphic and starts with $q$, so it is a normalized [cusp form](../../../../../cusp-form.md). The proof in Question 1 shows $S_{12}=\mathbb C\Delta_0$, giving $A^{24}=\Delta_0$. In particular $A$ has no interior zeros, by the [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md).

The [Serre derivative](../../../../../serre-derivative.md) argument in Question 2 gives $D\Delta_0=E_2\Delta_0$. Hence $DA/A=E_2/24$. The analytic product $P(\tau)=q^{1/24}\prod_{n\geq1}(1-q^n)$ is nonzero and has the same [logarithmic derivative](../../../../../logarithmic-derivative.md), since $DP/P=1/24-\sum\sigma_1(n)q^n$. Therefore $A/P$ is constant on the connected [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md); its limit at infinity is one. This proves $A=P$, without assuming either of the product identities being deduced. Pair the terms $n,-n$ in $A$, choosing representatives $n=6r+1$. Since $\chi_{12}(6r+1)=(-1)^r$, we get

$$
A=q^{1/24}\sum_{r\in\mathbb Z}(-1)^r q^{r(3r+1)/2},
\qquad
\boxed{\prod_{n\geq1}(1-q^n)=\sum_{r\in\mathbb Z}(-1)^r q^{r(3r+1)/2}.}
$$

This is the [Euler pentagonal identity](../../../../../euler-pentagonal-identity.md), derived by the [character theta proof of the eta product](../../../../../character-theta-proof-of-the-eta-product.md).

For the second product use the odd primitive character $\chi_4(1)=1$, $\chi_4(3)=-1$, with [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md) $2i$. Set

$$
B(\tau)=\tfrac12\widetilde\theta_{\chi_4}(\tau/4)=\tfrac12\sum_n n\chi_4(n)q^{n^2/8}.
$$

The odd transformation gives $B(-1/\tau)=(-i\tau)^{3/2}B(\tau)$ and the series gives $B(\tau+1)=e^{\pi i/4}B(\tau)$. Thus $B^8$ is another normalized weight-twelve [cusp form](../../../../../cusp-form.md), and $B^8=\Delta_0=A^{24}$. Because $A$ is nonzero, $B/A^3$ has eighth power one, so it is constant; its leading coefficient fixes it to one. Pairing positive and negative odd integers now gives

$$
B=q^{1/8}\sum_{r\geq0}(-1)^r(2r+1)q^{r(r+1)/2}.
$$

Since $B=A^3=q^{1/8}\prod_{n\geq1}(1-q^n)^3$, the [Jacobi cubic product identity](../../../../../jacobi-cubic-product-identity.md) follows:

$$
\boxed{\prod_{n\geq1}(1-q^n)^3=\sum_{r\geq0}(-1)^r(2r+1)q^{r(r+1)/2}.}
$$

All pairings and differentiations take place in locally uniformly convergent [theta functions](../../../../../theta-function.md) or products on $|q|<1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
