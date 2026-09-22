<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

First use independent fair signs $\varepsilon_i\in\{-1,1\}$, the [Rademacher distribution](../../../../../rademacher-distribution.md) convention for [Bernoulli random variables](../../../../../bernoulli-distribution.md) in this setting. Let $\Omega=\{-1,1\}^d$ with uniform [probability](../../../../../probability.md), write $s(\omega)=\sum_i\omega_i a_i$ and $F(\omega)=\|s(\omega)\|$. We prove the [sharp Rademacher second-moment inequality](../../../../../sharp-rademacher-second-moment-inequality.md) by a complete finite-cube calculation.

For a function on this cube define the [coordinate-flip generator on a hypercube](../../../../../coordinate-flip-generator-on-a-hypercube.md)

$$
Lu(\omega)=\frac12\sum_{i=1}^d
\bigl(u(\omega^{(i)})-u(\omega)\bigr),
$$

where $\omega^{(i)}$ flips just coordinate $i$. The [Walsh characters](../../../../../walsh-character.md) $\chi_A(\omega)=\prod_{i\in A}\omega_i$ form an [orthonormal basis](../../../../../orthonormal-basis.md): distinct characters have expectation-zero product, and there are $2^d$ of them. Flipping a coordinate in $A$ changes its sign and other flips leave it unchanged, so $L\chi_A=-|A|\chi_A$. Expand the real function $F$ as $\sum_A\widehat F(A)\chi_A$. Since $F(-\omega)=F(\omega)$, changing variables $\omega\mapsto-\omega$ shows that $\widehat F(A)=0$ whenever $|A|$ is odd. Thus

$$
-\mathbb E[FLF]=\sum_A|A|\widehat F(A)^2
\geq2\sum_{A\ne\varnothing}\widehat F(A)^2
=2\operatorname{Var}(F).
$$

This derives the [even-function spectral gap on a hypercube](../../../../../even-function-spectral-gap-on-a-hypercube.md), rather than assuming it.

At each vertex with $s(\omega)\ne0$, choose a [norming functional](../../../../../norming-functional.md) $\ell_\omega$ of [norm](../../../../../norm.md) one satisfying $\ell_\omega(s(\omega))=F(\omega)$, supplied by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). For complex $E$ take [real parts](../../../../../real-part.md) in the following inequalities. At a vertex with $s(\omega)=0$, use the zero functional. The supporting inequality for the [norm](../../../../../norm.md) gives

$$
F(\omega^{(i)})-F(\omega)
\geq\operatorname{Re}\ell_\omega
\bigl(s(\omega^{(i)})-s(\omega)\bigr).
$$

But $Ls=-s$, since every coefficient is a degree-one [Walsh character](../../../../../walsh-character.md). Summing the preceding inequalities with factor $1/2$ therefore proves $LF(\omega)\geq-F(\omega)$. As $F\geq0$,

$$
2\bigl(\mathbb EF^2-(\mathbb EF)^2\bigr)
\leq-\mathbb E[FLF]\leq\mathbb EF^2.
$$

Rearranging and taking [square roots](../../../../../square-root.md) yields

$$
\boxed{\left\|\sum_i\varepsilon_i a_i\right\|_{L^2(E)}
\leq\sqrt2\left\|\sum_i\varepsilon_i a_i\right\|_{L^1(E)}.}
$$

No completeness of $E$ is needed. The constant is sharp: with two identical nonzero scalar coefficients, the absolute sum is zero with [probability](../../../../../probability.md) $1/2$ and twice the coefficient magnitude with [probability](../../../../../probability.md) $1/2$.

If Bernoulli instead means fair $\{0,1\}$ variables $b_i$, write $b_i=(1+\varepsilon_i)/2$ and $a=\sum_i a_i$. Add an independent fair sign $\varepsilon_0$ and apply the proved estimate to $Y=\varepsilon_0a+\sum_i\varepsilon_i a_i$. Conditional on either sign of $\varepsilon_0$, $\|Y\|$ has the same distribution as $\|a+\sum_i\varepsilon_i a_i\|$, by symmetry of the sign sum. Hence $\|Y\|_{L^p(E)}=2\|\sum_i b_i a_i\|_{L^p(E)}$ for $p=1,2$, proving the same bound in that convention.

The constant is documented in [the primary sharp-constant study](https://www.impan.pl/en/publishing-house/journals-and-series/studia-mathematica/all/109/1/108398/on-the-best-constant-in-the-khinchin-kahane-inequality).

Fairness is essential. For a general $\{0,1\}$ [Bernoulli random variable](../../../../../bernoulli-distribution.md) with success [probability](../../../../../probability.md) $0<t<1/2$, a single nonzero scalar coefficient gives $L^2/L^1=1/\sqrt t>\sqrt2$. Thus the printed term cannot be read as permitting arbitrary Bernoulli [probabilities](../../../../../probability.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
