<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the full [modular group](../../../../../modular-group.md) $\Gamma=SL_2(\mathbb Z)$ and [integer](../../../../../integer.md) weight $k$, a [modular form](../../../../../modular-form.md) is a [holomorphic function](../../../../../holomorphic-function.md) on the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) satisfying

$$
f\left(\frac{a\tau+b}{c\tau+d}\right)=(c\tau+d)^k f(\tau)
\quad\text{for all }\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma,
$$

and [holomorphic](../../../../../complex-differentiability-at-a-point.md) at the cusp at infinity. Explicitly, periodicity under $\tau\mapsto\tau+1$ gives a [Fourier expansion of a modular form](../../../../../fourier-expansion-of-a-modular-form.md) in $q=e^{2\pi i\tau}$, and holomorphy at the cusp means $f=\sum_{n\geq0}a_nq^n$. A [cusp form](../../../../../cusp-form.md) has $a_0=0$. All cusps are equivalent for this group. The [matrix](../../../../../matrix.md) $-I$ forces $f=(-1)^kf$, so every odd-weight [modular form](../../../../../modular-form.md) is [zero](../../../../../zero-of-a-function.md).

There is a corresponding qualification to the displayed [Eisenstein series](../../../../../eisenstein-series.md) formula: **the Bernoulli-normalized formula is for even [integers](../../../../../integer.md) $k\geq4$.** For odd [integers](../../../../../integer.md) $k>2$, pairing $(m,n)$ with $(-m,-n)$ gives $G_k=0$, while $B_k=0$, so the printed expression divided by $B_k$ is undefined. We prove the asserted nonzero formula in its even-weight range.

On each [compact set](../../../../../compact-space.md) in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md), the real-linear map $(m,n)\mapsto m\tau+n$ has a uniformly bounded inverse. Hence $|m\tau+n|\geq C(m^2+n^2)^{1/2}$ there. For $k>2$, lattice convergence gives locally uniform [absolute convergence](../../../../../absolute-convergence.md) of $G_k$, and therefore holomorphy. If $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma$, then

$$
m\gamma\tau+n=\frac{(ma+nc)\tau+(mb+nd)}{c\tau+d}.
$$

The map $(m,n)\mapsto(ma+nc,mb+nd)$ permutes the nonzero [integer](../../../../../integer.md) pairs. Reindexing proves the weight-$k$ transformation law.

To compute the [Fourier expansion of a normalized Eisenstein series](../../../../../fourier-expansion-of-a-normalized-eisenstein-series.md), start from the [cotangent partial-fraction expansion](../../../../../cotangent-partial-fraction-expansion.md)

$$
\pi\cot(\pi z)=\frac1z+\sum_{n\geq1}\left(\frac1{z+n}+\frac1{z-n}\right).
$$

For $\operatorname{Im}z>0$, the [cotangent Fourier expansion](../../../../../cotangent-fourier-expansion.md) is $\pi\cot(\pi z)=-\pi i-2\pi i\sum_{r\geq1}e^{2\pi irz}$. Differentiating both normally convergent expressions $k-1$ times gives

$$
\sum_{n\in\mathbb Z}(z+n)^{-k}=\frac{(-2\pi i)^k}{(k-1)!}\sum_{r\geq1}r^{k-1}e^{2\pi irz}.
$$

For even $k$, the terms with $m=0$ sum to $2\zeta(k)$, and the terms with $m<0$ duplicate those with $m>0$. Substituting $z=m\tau$ in the last identity and collecting $N=mr$ gives

$$
G_k(\tau)=2\zeta(k)+\frac{2(2\pi i)^k}{(k-1)!}\sum_{N\geq1}\sigma_{k-1}(N)q^N,
\qquad
\sigma_{k-1}(N)=\sum_{d\mid N}d^{k-1}.
$$

The rearrangement is absolutely convergent for every $|q|<1$, since the [divisor function](../../../../../divisor-function.md) grows at most polynomially.

For completeness, the normalization follows directly from the definition of the [Bernoulli numbers](../../../../../bernoulli-number.md). Near [zero](../../../../../zero-of-a-function.md), the [cotangent partial-fraction expansion](../../../../../cotangent-partial-fraction-expansion.md) gives

$$
\pi\cot(\pi z)=z^{-1}-2\sum_{r\geq1}\zeta(2r)z^{2r-1}.
$$

On the other hand $\pi\cot(\pi z)=\pi i+2\pi i/(e^{2\pi iz}-1)$. Substitute $t=2\pi iz$ in the generating function of the [Bernoulli numbers](../../../../../bernoulli-number.md). The term $B_1=-1/2$ cancels $\pi i$, and the higher odd terms vanish because $t/(e^t-1)+t/2$ is even. Comparison of [Laurent coefficients](../../../../../laurent-coefficient.md) proves the [Euler evaluation of even zeta values](../../../../../euler-evaluation-of-even-zeta-values.md)

$$
2\zeta(k)=-\frac{B_k(2\pi i)^k}{k!}\quad(k\text{ even},\ k\geq2).
$$

Thus

$$
\boxed{G_k(\tau)=2\zeta(k)\left(1-\frac{2k}{B_k}\sum_{n\geq1}\sigma_{k-1}(n)q^n\right),\qquad k\geq4\text{ even}.}
$$

This [Fourier series](../../../../../fourier-series-split.md) also proves holomorphy at infinity, completing the [modular form](../../../../../modular-form.md) verification.

For the [Ramanujan congruence modulo 691](../../../../../ramanujan-congruence-modulo-691.md), the standard facts we use are that the [modular discriminant](../../../../../modular-discriminant.md) is the weight-twelve [cusp form](../../../../../cusp-form.md) $\Delta=q\prod_{n\geq1}(1-q^n)^{24}=\sum_{n\geq1}\tau(n)q^n$, and that $S_{12}=\mathbb C\Delta$. The latter also follows from the [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md): a nonzero weight-twelve [modular form](../../../../../modular-form.md) has total weighted [zero](../../../../../zero-of-a-function.md) order one, so a [cusp form](../../../../../cusp-form.md) whose coefficient of $q$ vanishes would have cusp order at least two and must be [zero](../../../../../zero-of-a-function.md). The product makes the [Ramanujan tau function](../../../../../ramanujan-tau-function.md) integer-valued.

Write $E_k=G_k/(2\zeta(k))$. Using $B_4=-1/30$ and the supplied $B_{12}=-691/2730$, we have

$$
E_4=1+240\sum_{n\geq1}\sigma_3(n)q^n,\qquad
E_{12}=1+\frac{65520}{691}\sum_{n\geq1}\sigma_{11}(n)q^n.
$$

Both $E_{12}$ and $E_4^3$ have weight twelve and constant term one. Their difference is a [cusp form](../../../../../cusp-form.md), so is a multiple of $\Delta$. Its coefficient of $q$ is $65520/691-720=-432000/691$, which determines that multiple:

$$
691E_{12}=691E_4^3-432000\Delta.
$$

The coefficients of $E_4^3$ are [integers](../../../../../integer.md). Comparing the positive-index [Fourier coefficients](../../../../../fourier-coefficient.md) and reducing modulo $691$ therefore gives $65520\sigma_{11}(n)\equiv-432000\tau(n)$. Both numerical constants are congruent to $566$ modulo $691$, and $\gcd(566,691)=1$. Cancellation proves

$$
\boxed{\tau(n)\equiv\sigma_{11}(n)\pmod{691}\quad(n\geq1).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
