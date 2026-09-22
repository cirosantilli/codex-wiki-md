<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We use the [canonical height pairing](../../../../../../canonical-height-pairing.md) normalization $\langle P,Q\rangle=(\widehat h(P+Q)-\widehat h(P)-\widehat h(Q))/2$, so that $\langle P,P\rangle=\widehat h(P)$. The supplied values give

$$
\boxed{\langle P,Q\rangle\approx\frac{21.98-6.61-7.87}{2}=3.75.}
$$

The convention without the factor $1/2$ instead gives the doubled pairing $B(P,Q)\approx7.50$; all independence conclusions are the same.

In our convention the [Gram matrix](../../../../../../gram-matrix.md) is approximately

$$
H=\begin{pmatrix}6.61&3.75\\3.75&7.87\end{pmatrix},\qquad
\det H\approx6.61\cdot7.87-3.75^2=37.9582>0.
$$

This positive margin is much larger than the rounding uncertainty. Even allowing each of the three stated heights an error of $0.01$, we have $a\geq6.60$, $b\geq7.86$ and $|c|\leq3.765$, giving $ab-c^2\geq6.60\cdot7.86-3.765^2=37.700775>0$. Thus the actual [canonical height pairing](../../../../../../canonical-height-pairing.md) matrix is [positive-definite](../../../../../../positive-definite-bilinear-form.md), not merely its rounded approximation.

If $rP+sQ=O$ for integers $r,s$, [bilinearity](../../../../../../bilinearity.md) and the [height parallelogram identity](../../../../../../height-parallelogram-identity.md) give $0=\widehat h(rP+sQ)=ar^2+2crs+bs^2$. Positive definiteness forces $r=s=0$. This is the [rank certificate from rounded canonical heights](../../../../../../rank-certificate-from-rounded-canonical-heights.md), and proves

$$
\boxed{\langle P,Q\rangle_{\mathrm{group}}\cong\mathbb Z\times\mathbb Z.}
$$

Here the last brackets denote the generated subgroup, not the scalar height pairing. The argument proves independence; it does not assert that these points generate the entire [Mordell-Weil group](../../../../../../mordell-weil-group.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
