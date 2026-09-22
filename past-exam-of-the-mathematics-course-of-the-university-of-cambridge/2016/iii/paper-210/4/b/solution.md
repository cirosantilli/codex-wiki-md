<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [symmetric matrix](../../../../../../symmetric-matrix.md) $H$ with simple largest [eigenvalue](../../../../../../eigenvalue.md) and [spectral gap](../../../../../../spectral-gap.md) $\gamma$, the [Davis-Kahan curvature lemma](../../../../../../davis-kahan-curvature-lemma.md) says $\frac\gamma2\|uu^\top-vv^\top\|_F^2\leq\operatorname{tr}(H(vv^\top-uu^\top))$, where $v$ is its leading unit [eigenvector](../../../../../../eigenvector.md). Applying this to a leading [eigenvector](../../../../../../eigenvector.md) $\widehat v$ of $H+W$, the maximal [Rayleigh quotient](../../../../../../rayleigh-quotient.md) and duality of the [operator norm](../../../../../../operator-norm.md) and [trace norm](../../../../../../trace-norm.md) give $\|\widehat v\widehat v^\top-vv^\top\|_F\leq2\sqrt2\|W\|_{\mathrm{op}}/\gamma$; the projector difference has [matrix rank](../../../../../../matrix-rank.md) at most two. This is a [rank-one eigenprojector perturbation bound](../../../../../../rank-one-eigenprojector-perturbation-bound.md).

Here $W=M-M_0=A-A_0$ has independent centered bounded upper-triangular entries, apart from symmetry. The [spectral norm bound for a centered Bernoulli adjacency matrix](../../../../../../spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix.md) gives $\mathbb E\|W\|_{\mathrm{op}}\leq C_0\sqrt n$. Taking $H=M_0$ and $\gamma=t\sqrt n/2$ therefore gives, **for the largest-eigenvalue estimator**,

$$
\boxed{\mathbb E\|\widehat v\widehat v^\top-vv^\top\|_F\leq\frac{4\sqrt2 C_0}{t}.}
$$

**The printed argmin selects the wrong end of the spectrum.** For a minimizing unit [eigenvector](../../../../../../eigenvector.md) $u$, compare its [Rayleigh quotient](../../../../../../rayleigh-quotient.md) with any unit vector orthogonal to $v$. This yields $\gamma|u^\top v|^2\leq2\|W\|_{\mathrm{op}}$, and hence $\mathbb E|u^\top v|^2\leq4C_0/t$. Its mean projector error is at least $\sqrt2(1-4C_0/t)$, using $\sqrt{1-x}\geq1-x$. Along $t=n^{1/4}$ with sufficiently large even $n$, the printed parameter restriction holds and this lower bound tends to $\sqrt2$, contradicting an error of order $1/t$. Replace argmin by argmax, or negate the entire matrix before minimizing.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
