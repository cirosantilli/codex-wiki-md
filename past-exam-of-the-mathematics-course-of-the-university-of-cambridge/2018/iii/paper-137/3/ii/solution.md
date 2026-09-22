<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the convention that a [weak modular form](../../../../../../weak-modular-form.md) is a [holomorphic function](../../../../../../holomorphic-function.md) $f$ on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) satisfying

$$
f(\gamma z)=(cz+d)^k f(z)\quad(\gamma\in SL_2(\mathbb Z)),
$$

with no condition at infinity. In particular $f(z+1)=f(z)$, so it has a [Laurent series](../../../../../../laurent-series.md) $f(z)=\sum_{n\in\mathbb Z}a_nq^n$ on $0<|q|<1$, where $q=e^{2\pi iz}$. It is a [modular form](../../../../../../modular-form.md) when it is [holomorphic at a cusp](../../../../../../holomorphic-at-a-cusp.md), here the unique level-one cusp at infinity, equivalently $a_n=0$ for $n<0$. It is a [cusp form](../../../../../../cusp-form.md) when additionally $a_0=0$. If one uses the narrower weakly [holomorphic](../../../../../../complex-differentiability-at-a-point.md) convention, one also requires finitely many negative terms; the derivative argument below holds in that subspace as well. The matrix $-I$ forces odd-weight forms to be zero.

Put $(a)_r=a(a+1)\cdots(a+r-1)$, with $(a)_0=1$, and

$$
C_{\ell,j}=\binom\ell j(k+j)_{\ell-j}\quad(0\leq j\leq\ell).
$$

We prove the [derivative transformation of a weak modular form](../../../../../../derivative-transformation-of-a-weak-modular-form.md) in the uniform form

$$
f^{(\ell)}(-1/z)=\sum_{j=0}^{\ell}C_{\ell,j}z^{k+\ell+j}f^{(j)}(z).
$$

For $\ell=0$ this is the weight-$k$ transformation under $S$. Differentiating the formula and multiplying by $z^2$, since $d(-1/z)/dz=z^{-2}$, gives the recurrence

$$
C_{\ell+1,j}=(k+\ell+j)C_{\ell,j}+C_{\ell,j-1},
$$

where out-of-range coefficients are zero. The displayed explicit coefficients satisfy it. Indeed, for interior $j$, extract the common polynomial $(k+j)_{\ell-j}$; the remaining identity is

$$
\binom\ell j(k+\ell+j)+\binom\ell{j-1}(k+j-1)
=\binom{\ell+1}j(k+\ell).
$$

This follows from [Pascal's identity](../../../../../../pascal-s-rule.md) and $j\binom\ell j=(\ell-j+1)\binom\ell{j-1}$. The endpoint coefficients satisfy the recurrence directly. This polynomial proof also applies when a factor is zero, avoiding division by that factor. As $C_{\ell,\ell}=1$, the result is

$$
\boxed{f^{(\ell)}(-1/z)=z^{k+2\ell}f^{(\ell)}(z)
+\sum_{j=0}^{\ell-1}\binom\ell j(k+\ell-1)\cdots(k+j)
 z^{k+\ell+j}f^{(j)}(z).}
$$

The letter $l$ in the printed exponent is the same derivative order $\ell$.

For integer $k<0$, take $\ell=1-k$. If $j<\ell$, the product runs from $k+j\leq0$ through $k+\ell-1=0$, and therefore vanishes. Consequently $f^{(1-k)}$ has weight $k+2(1-k)=2-k$ under $S$. It is also invariant under $T$, by differentiating $f(z+1)=f(z)$, and $S,T$ generate the [modular group](../../../../../../modular-group.md). Its holomorphy is preserved by differentiation. With $D=(2\pi i)^{-1}d/dz=q\,d/dq$, termwise differentiation of the locally convergent [Laurent series](../../../../../../laurent-series.md) gives the [Bol identity for modular forms](../../../../../../bol-identity-for-modular-forms.md):

$$
\boxed{D^{1-k}f=\sum_{n\in\mathbb Z}n^{1-k}a_nq^n
\text{ is a weak modular form of weight }2-k.}
$$

For negative indices the exponent $1-k$ is a positive integer, and the constant term is killed, so every term is unambiguous.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
