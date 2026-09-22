<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Dolbeault theorem](../../../../../../dolbeault-theorem.md) identifies $H^2(M,\mathcal O_M)$ with $H^{0,2}_{\bar\partial}(M)$. It vanishes by hypothesis, and [complex conjugation](../../../../../../complex-conjugation.md) in the [Hodge decomposition theorem for compact Kähler manifolds](../../../../../../hodge-decomposition-theorem-for-compact-kahler-manifolds.md) makes $H^{2,0}$ vanish too. Thus every real degree-two cohomology class has type $(1,1)$.

Let $\omega$ be a Kähler form. Choose a rational cohomology class $\eta$ sufficiently close to $[\omega]$. More concretely, using [harmonic differential forms](../../../../../../harmonic-differential-form.md) as representatives for a fixed [Kähler metric](../../../../../../kahler-metric.md), the harmonic form representing $\eta$ is close to $\omega$ in every smooth norm: [harmonic differential forms](../../../../../../harmonic-differential-form.md) constitute a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md). It is a real closed $(1,1)$ form, and is positive if sufficiently close to $\omega$, by [compactness](../../../../../../compact-space.md). This is the openness of the [Kähler cone](../../../../../../kahler-cone.md). Multiplying by a positive integer gives an integral Kähler class $\kappa=N\eta$.

The [holomorphic exponential sequence](../../../../../../holomorphic-exponential-sequence.md) contains the cohomology segment

$$
H^1(M,\mathcal O_M^*)\xrightarrow{c_1}H^2(M,\mathbb Z)\longrightarrow H^2(M,\mathcal O_M)=0.
$$

Choose an integral lift of $\kappa$. Exactness gives a [holomorphic line bundle](../../../../../../holomorphic-line-bundle.md) $\mathcal L$ having that [First Chern class](../../../../../../first-chern-class.md). We must ensure that it has a positive metric, rather than merely a positive representative of its class.

Choose any [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) $h_0$ and let $\theta_0$ be its [normalized curvature form of a Hermitian holomorphic line bundle](../../../../../../normalized-curvature-form-of-a-hermitian-holomorphic-line-bundle.md). If $\theta$ is the positive form representing $\kappa$, then $\theta-\theta_0$ is an exact real $(1,1)$ form. The [ddbar lemma](../../../../../../ddbar-lemma.md) gives a real smooth function $u$ with

$$
\theta-\theta_0=\frac{i}{2\pi}\partial\bar\partial u.
$$

Replace $h_0$ by $h=e^{-u}h_0$. Its normalized curvature is $\theta$, so $\mathcal L$ is a [positive holomorphic line bundle](../../../../../../positive-holomorphic-line-bundle.md). The [Kodaira embedding theorem](../../../../../../kodaira-embedding-theorem.md) now applies: sufficiently many sections of a sufficiently high [tensor power](../../../../../../tensor-power.md) define the desired embedding. Therefore

$$
\boxed{H^2(M,\mathcal O_M)=0\ \Longrightarrow\ M\text{ admits a holomorphic embedding into complex projective space}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
