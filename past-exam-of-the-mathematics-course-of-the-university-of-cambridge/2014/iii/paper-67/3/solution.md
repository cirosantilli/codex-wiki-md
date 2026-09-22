<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $D_j=-i\partial_{x_j}$, so the [Fourier transform](../../../../../fourier-transform.md) of $D^\alpha u$ is $\lambda^\alpha\widehat u$. Distinguish the full degree-$N$ [polynomial](../../../../../polynomial-split.md) $P(\lambda)$ from its homogeneous top-degree part $p_N(\lambda)$, the [principal symbol](../../../../../principal-symbol-of-a-partial-differential-equation.md). The [elliptic differential operator](../../../../../elliptic-differential-operator.md) condition is

$$
\boxed{p_N(\lambda)\ne0\quad\text{for every real }\lambda\ne0.}
$$

It does not require the full [polynomial](../../../../../polynomial-split.md) to be nonzero at small frequencies. Compactness of the unit sphere gives $c_0=\min_{|\theta|=1}|p_N(\theta)|>0$. Homogeneity and the lower-degree remainder imply

$$
|P(\lambda)|\ge c_0|\lambda|^N-C(1+|\lambda|)^{N-1}.
$$

For sufficiently large $|\lambda|$ the second term is at most half the first, so the [high-frequency lower bound for an elliptic polynomial](../../../../../high-frequency-lower-bound-for-an-elliptic-polynomial.md) is

$$
\boxed{|P(\lambda)|\ge c\langle\lambda\rangle^N,}
\qquad\langle\lambda\rangle=(1+|\lambda|^2)^{1/2}.
$$

Here $\langle\lambda\rangle$ is the [Japanese bracket](../../../../../japanese-bracket.md). The order-zero case just means a nonzero constant and is immediate.

For real $s$, the [Sobolev space](../../../../../sobolev-space-split.md) definition with the current Fourier normalization is

$$
H^s(\mathbb R^n)=\{u\in\mathcal S':\langle\lambda\rangle^s\widehat u\in L^2\},
\qquad\|u\|_{H^s}^2=(2\pi)^{-n}\int\langle\lambda\rangle^{2s}|\widehat u(\lambda)|^2\,d\lambda.
$$

Changing the harmless constant in the norm gives the same space. A [distribution](../../../../../distribution-mathematical-analysis.md) on $X$ belongs to the [Local Sobolev space](../../../../../local-sobolev-space.md) $H^s_{\rm loc}(X)$ when $\chi u$, extended by zero outside $X$, belongs to $H^s(\mathbb R^n)$ for every [test function](../../../../../test-function.md) $\chi\in C_c^\infty(X)$.

A [compactly supported distribution](../../../../../compactly-supported-distribution.md) of finite [order of a distribution](../../../../../order-of-a-distribution.md) $m$ has a smooth [Fourier transform](../../../../../fourier-transform.md) satisfying $|\widehat u(\lambda)|\le C(1+|\lambda|)^m$, by applying the finite-order estimate to a fixed cutoff times the exponential. Thus its weighted squared transform is bounded by $C\langle\lambda\rangle^{2(s+m)}$. This is integrable precisely in the sufficient range $2(s+m)<-n$, and proves

$$
\boxed{u\in H^s(\mathbb R^n)\quad\text{for every }s<-m-n/2.}
$$

This is the [negative Sobolev regularity of a compactly supported distribution](../../../../../negative-sobolev-regularity-of-a-compactly-supported-distribution.md); the strict inequality is important, and is not a claim that this sufficient threshold is optimal for each [distribution](../../../../../distribution-mathematical-analysis.md).

To establish [elliptic regularity](../../../../../elliptic-regularity.md) without assuming the answer as an a priori smoothness hypothesis, first obtain a global constant-coefficient gain. For a compactly supported [distribution](../../../../../distribution-mathematical-analysis.md) $w$ with $P(D)w\in H^q$, the [polynomial](../../../../../polynomial-split.md) lower bound at high frequency gives

$$
\int_{|\lambda|\ge R}\langle\lambda\rangle^{2(q+N)}|\widehat w|^2\,d\lambda
\le C\int_{|\lambda|\ge R}\langle\lambda\rangle^{2q}|\widehat{P(D)w}|^2\,d\lambda<\infty.
$$

On $|\lambda|\le R$, the transform of $w$ is smooth and bounded. Therefore **$P(D)w\in H^q$ implies $w\in H^{q+N}$**. Possible low-frequency zeros of $P$ are harmless; we never divide by them.

Two elementary mapping facts supply the variable-coefficient argument. [Distributional derivatives](../../../../../distributional-derivative.md) of order $j$ map $H^r$ into $H^{r-j}$. [Sobolev multiplication by a smooth cutoff](../../../../../sobolev-multiplication-by-a-smooth-cutoff.md) is bounded on $H^r$ for every real $r$, including negative ones. Indeed, for a compactly supported smooth $a$, the [Peetre weight inequality](../../../../../peetre-weight-inequality.md)

$$
\langle\xi\rangle^r\le C_r\langle\eta\rangle^r\langle\xi-\eta\rangle^{|r|}
$$

and $\widehat{aw}=(2\pi)^{-n}\widehat a*\widehat w$ reduce the bound to [Young's convolution inequality](../../../../../young-s-convolution-inequality.md) with the integrable kernel $\langle\zeta\rangle^{|r|}|\widehat a(\zeta)|$. Smooth coefficients only need this property on compact subsets, where they can be multiplied by another cutoff.

Write the lower-order part as $B=\sum_{|\alpha|<N}f_\alpha D^\alpha$, with $N\ge1$, and suppose provisionally that $u\in H^r_{\rm loc}$ on a relatively compact neighborhood. For a [cutoff function](../../../../../cutoff-function.md) $\chi$ supported there,

$$
P(D)(\chi u)=\chi Lu-\chi Bu+[P(D),\chi]u.
$$

The bracket is the operator [commutator](../../../../../commutator.md). Its order is at most $N-1$: in the product rule, every surviving term has at least one derivative falling on $\chi$. Choose a second [cutoff function](../../../../../cutoff-function.md) equal to one near $\operatorname{supp}\chi$ when estimating the products. The derivative and smooth-multiplication bounds then give

$$
\chi Bu,\ [P(D),\chi]u\in H^{r-N+1},\qquad \chi Lu\in H^s.
$$

The global gain just proved applies to the [compactly supported distribution](../../../../../compactly-supported-distribution.md) $\chi u$, and yields

$$
\boxed{u\in H^{\min(s+N,r+1)}_{\rm loc}.}
$$

This is the [cutoff bootstrap for local elliptic regularity](../../../../../cutoff-bootstrap-for-local-elliptic-regularity.md); it works for real indices, not just nonnegative integers.

There is always a legitimate starting index. Around any fixed point choose $\chi_0=1$ on a smaller neighborhood. The [compactly supported distribution](../../../../../compactly-supported-distribution.md) $\chi_0u$ has the negative Sobolev regularity proved above, so $u\in H^{r_0}_{\rm loc}$ on that neighborhood for some finite $r_0$. The index need not be uniform over all of $X$. Repeating the one-step gain finitely many times reaches $s+N$, or the target is already reached if $r_0\ge s+N$. Since the point was arbitrary,

$$
\boxed{Lu\in H^s_{\rm loc}(X)\ \Longrightarrow\ u\in H^{s+N}_{\rm loc}(X).}
$$

For $N=0$ the result follows directly by dividing by the nonzero constant.

Finally, if $Lu=0$, its forcing belongs to every [Local Sobolev space](../../../../../local-sobolev-space.md). The gain consequently gives every local Sobolev order for $u$. For each integer $j\ge0$, choose an order larger than $j+n/2$ and apply the [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md) to a localized solution. It has a $C^j$ representative; the representatives agree because they represent the same [distribution](../../../../../distribution-mathematical-analysis.md). Thus **every distributional solution of $Lu=0$ is smooth on $X$**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
