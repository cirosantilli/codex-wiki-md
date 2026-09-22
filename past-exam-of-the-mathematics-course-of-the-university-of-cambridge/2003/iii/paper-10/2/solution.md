<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We use independent symmetric [Rademacher random variables](../../../../../rademacher-distribution.md) $\varepsilon_j\in\{-1,1\}$, the intended meaning of the Bernoulli variables in this context. Without this convention the assertion need not hold: for one $0/1$ Bernoulli variable of success probability $t<1/2$ and one nonzero vector, the proposed inequality would be $\sqrt t\le\sqrt2\,t$, which is false.

Let $\Omega=\{-1,1\}^n$ with the uniform [probability measure](../../../../../probability-measure.md), put $S(\varepsilon)=\sum_j\varepsilon_jx_j$, and set $F(\varepsilon)=\|S(\varepsilon)\|$. We prove the sharp estimate rather than assuming the [Kahane-Khintchine inequality](../../../../../kahane-khintchine-inequality.md). If $\varepsilon^{(j)}$ denotes $\varepsilon$ with its $j$th sign reversed, define

$$
\mathcal Lf(\varepsilon)=\frac12\sum_{j=1}^n\bigl(f(\varepsilon^{(j)})-f(\varepsilon)\bigr).
$$

The [Walsh characters](../../../../../walsh-character.md) $w_A(\varepsilon)=\prod_{j\in A}\varepsilon_j$ form an [orthonormal basis](../../../../../orthonormal-basis.md) of scalar functions on this finite cube, and $\mathcal Lw_A=-|A|w_A$. Since $F(-\varepsilon)=F(\varepsilon)$, its coefficients for odd $|A|$ vanish. Every nonconstant remaining character has $|A|\ge2$. Expanding in this [orthonormal basis](../../../../../orthonormal-basis.md) gives the [even-function spectral gap on a hypercube](../../../../../even-function-spectral-gap-on-a-hypercube.md)

$$
2\bigl(\mathbb EF^2-(\mathbb EF)^2\bigr)\le\mathbb E\bigl[F(-\mathcal LF)\bigr].
$$

At each $\varepsilon$, the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) supplies a real norming [linear functional](../../../../../linear-functional.md) $\phi$ with $\|\phi\|\le1$ and $\phi(S(\varepsilon))=F(\varepsilon)$. For a complex [Banach space](../../../../../banach-space-split.md) use its underlying real space. Since $\|z\|\ge\phi(z)$,

$$
F(\varepsilon^{(j)})-F(\varepsilon)\ge-2\phi(\varepsilon_jx_j).
$$

Adding gives $\mathcal LF\ge-F$. Multiplying by the nonnegative $F$ yields $F(-\mathcal LF)\le F^2$. Therefore

$$
2\bigl(\mathbb EF^2-(\mathbb EF)^2\bigr)\le\mathbb EF^2,
\qquad
\boxed{\left(\mathbb E\left\|\sum_j\varepsilon_jx_j\right\|^2\right)^{1/2}\le\sqrt2\,\mathbb E\left\|\sum_j\varepsilon_jx_j\right\|.}
$$

The constant is sharp: take $n=2$ and $x_1=x_2\ne0$ in the scalar field. The random norm is $0$ or $2\|x_1\|$, each with probability one half.

A [Banach space](../../../../../banach-space-split.md) has [cotype 2](../../../../../cotype-2.md) if a constant $C$, independent of the length of the family, satisfies

$$
\left(\sum_j\|x_j\|^2\right)^{1/2}\le C\left(\mathbb E\left\|\sum_j\varepsilon_jx_j\right\|^2\right)^{1/2}.
$$

For $f_j\in L^1(0,1)$, the [triangle inequality](../../../../../triangle-inequality.md) for the Euclidean norm gives

$$
\left(\sum_j\|f_j\|_1^2\right)^{1/2}
=\left\|\int_0^1(|f_j(t)|)_j\,dt\right\|_2
\le\int_0^1\left(\sum_j|f_j(t)|^2\right)^{1/2}\,dt.
$$

For real or complex scalars $a_j$, independence gives $\mathbb E|\sum_j\varepsilon_ja_j|^2=\sum_j|a_j|^2$. The proved [sharp Rademacher second-moment inequality](../../../../../sharp-rademacher-second-moment-inequality.md), applied pointwise to $(f_j(t))$, and [Fubini theorem](../../../../../fubini-s-theorem.md) now yield

$$
\left(\sum_j\|f_j\|_1^2\right)^{1/2}
\le\sqrt2\int_0^1\mathbb E\left|\sum_j\varepsilon_jf_j(t)\right|\,dt
=\sqrt2\,\mathbb E\left\|\sum_j\varepsilon_jf_j\right\|_1
\le\sqrt2\left(\mathbb E\left\|\sum_j\varepsilon_jf_j\right\|_1^2\right)^{1/2}.
$$

Thus **$L^1(0,1)$ has cotype 2, with $C\le\sqrt2$**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
