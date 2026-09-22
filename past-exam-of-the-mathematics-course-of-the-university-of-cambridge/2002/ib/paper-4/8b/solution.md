<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Use $\widehat f(t)=\int f(x)e^{-itx}\,dx$ and its extension to [square-integrable functions](../../../../../square-integrable-function.md). For $T_kf(x)=f(x+k)$, changing variables gives $\widehat{T_kf}(t)=e^{ikt}\widehat f(t)$. The [Plancherel theorem](../../../../../plancherel-theorem.md) therefore gives

$$
\int_{\mathbb R}f(x+k)\overline{f(x+l)}\,dx=\frac1{2\pi}\int_{\mathbb R}|\widehat f(t)|^2e^{i(k-l)t}\,dt.
$$

For an arbitrary square-integrable $f$, the translation identity follows by approximation by integrable square-integrable functions: translations are isometries in $L^2$ and the [Fourier transform](../../../../../fourier-transform.md) is continuous in the Plancherel [norm](../../../../../norm.md). The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) makes the product on the left integrable, and $|\widehat f|^2$ is integrable on the right.

Put $m=l-k$. Every unequal integer pair gives a nonzero integer $m$, and every nonzero integer arises, for example with $k=0,l=m$. The identity thus proves **both directions of the requested equivalence**. It is the [orthogonality of integer translates](../../../../../orthogonality-of-integer-translates.md) criterion. A different Fourier normalization changes only the nonzero constant factor, not the vanishing conditions.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
