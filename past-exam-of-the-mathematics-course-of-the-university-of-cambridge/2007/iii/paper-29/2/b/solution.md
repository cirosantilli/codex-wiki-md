<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A weight-$2k$ [modular form](../../../../../../modular-form.md) gives an invariant tensor differential

$$
\omega_f=f(\tau)(d\tau)^k,
$$

because $d(\gamma\tau)=(c\tau+d)^{-2}d\tau$ cancels its [automorphy factor](../../../../../../automorphy-factor.md). Assume first $k\geq0$. At an ordinary quotient point this differential is [holomorphic](../../../../../../complex-differentiability-at-a-point.md). At an [elliptic point](../../../../../../elliptic-point.md) of order $e$, use $u$ and $w=u^e$ from part (a), and write the pullback as $A(u)(du)^k$, with $A$ [holomorphic](../../../../../../complex-differentiability-at-a-point.md). Its invariance says $A(\zeta u)\zeta^k=A(u)$, so a nonzero term $a_ru^r$ has $r+k\equiv0\pmod e$. Since

$$
u^r(du)^k=\frac1{e^k}u^{r-k(e-1)}(dw)^k,
$$

the exponent in the descended coefficient is the integer $(r-k(e-1))/e$. With $r\geq0$, it is at least $-\lfloor k(e-1)/e\rfloor$. At the [modular cusp](../../../../../../cusp-of-a-modular-group.md), $d\tau=dq/(2\pi iq)$ and $f$ has a power [series](../../../../../../series-mathematics.md) with nonnegative exponents, so $\omega_f$ has a [pole](../../../../../../pole.md) of order at most $k$.

Consequently the [linear map](../../../../../../linear-map.md) $f\mapsto\omega_f$ injects $M_{2k}$ into the [meromorphic](../../../../../../meromorphic-function.md) sections of $K^{\otimes k}$ with poles bounded by

$$
D=k[\infty]+\lfloor k/2\rfloor[i]+\lfloor2k/3\rfloor[\rho].
$$

This section space is $H^0(X(1),K^{\otimes k}(D))$. It is finite-dimensional on a [compact Riemann surface](../../../../../../compact-riemann-surface.md) by the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md). Concretely choose one nonzero [meromorphic](../../../../../../meromorphic-function.md) section of the line bundle; dividing by it identifies these sections with a [Riemann-Roch space](../../../../../../riemann-roch-space.md) with a fixed finite [divisor](../../../../../../divisor.md) bound. This proves the requested finite-dimensionality by compact-surface theory.

In fact the injection is an isomorphism. If a descended coefficient has order at least $-\lfloor k(e-1)/e\rfloor$, its pulled-back exponent $ed+k(e-1)$ is nonnegative; the [modular cusp](../../../../../../cusp-of-a-modular-group.md) [pole](../../../../../../pole.md) bound likewise gives a [holomorphic](../../../../../../complex-differentiability-at-a-point.md) [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md). These pullbacks therefore recover [modular forms](../../../../../../modular-form.md). Since $X(1)$ is the [Riemann sphere](../../../../../../riemann-sphere.md), $\deg K=-2$, and a line bundle of degree $d$ on the sphere has $\max(0,d+1)$ sections. Hence

$$
\boxed{\dim M_{2k}=\max\left(0,1-k+\left\lfloor\frac{k}{2}\right\rfloor+\left\lfloor\frac{2k}{3}\right\rfloor\right)\quad(k\geq0).}
$$

For negative $k$, the valence formula excludes a nonzero [holomorphic](../../../../../../complex-differentiability-at-a-point.md) [modular form](../../../../../../modular-form.md) because all its orders would be nonnegative but their sum would be $k/6<0$; the space is zero. The mechanism behind finite-dimensionality is [modular forms as meromorphic differentials on X(1)](../../../../../../modular-forms-as-meromorphic-differentials-on-x-1.md), with explicit elliptic and [modular cusp](../../../../../../cusp-of-a-modular-group.md) [pole](../../../../../../pole.md) bounds.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
