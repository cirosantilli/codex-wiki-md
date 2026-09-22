<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The entries in (b) satisfy

$$
|g_{ii}|-\sum_{j\ne i}|g_{ij}|\ge\frac23-\frac{h_i+h_{i+1}}{3(h_i+h_{i+1})}=\frac13.
$$

Thus $G$ has [strict diagonal dominance](../../../../../../strictly-diagonally-dominant-matrix.md) with margin at least $1/3$. To prove the [inverse infinity-norm bound from diagonal dominance](../../../../../../inverse-infinity-norm-bound-from-diagonal-dominance.md) directly, choose $i$ with $|a_i|=\|a\|_{\ell^\infty}$. The [reverse triangle inequality](../../../../../../reverse-triangle-inequality.md) gives

$$
\|Ga\|_{\ell^\infty}\ge|(Ga)_i|\ge\left(|g_{ii}|-\sum_{j\ne i}|g_{ij}|\right)|a_i|\ge\frac13\|a\|_{\ell^\infty}.
$$

This also proves that the [kernel](../../../../../../kernel-of-a-linear-map.md) is zero and hence that $G$ is invertible. Substituting $a=G^{-1}b$ and taking the [operator norm](../../../../../../operator-norm.md) gives

$$
\boxed{\|G^{-1}\|_{\ell^\infty}\le3}.
$$

Combined with (a), it yields $\|P_S\|_\infty\le3$ for linear [splines](../../../../../../spline-mathematics.md), independently of the knot spacings. The diagonal-dominance argument already proves the required estimate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
