# Cholesky decomposition and geodetic adjustment

↑ **Parent:** [Cholesky decomposition](cholesky-decomposition.md)

[André-Louis Cholesky](andre-louis-cholesky.md) developed his calculation in the setting of geodetic adjustment: measured angles and lengths must satisfy geometric relations, while corrections should be small. The manuscript reproduced in [Claude Brezinski](claude-brezinski.md)'s study is titled Sur la résolution numérique des systèmes d’équations linéaires and ends with the date 2 December 1910 at Vincennes. The manuscript reports a 56-equation calculation adjusting altitudes in an Algerian triangulation network. Its date establishes when this written account existed, rather than an exact invention date.[Claude Brezinski, La méthode de Cholesky, printed pp. 210–211: geodetic least-squares corrections; p. 217: manuscript title and caution about invention date; §4, p. 229: reproduced manuscript's 56-equation adjustment and closing date](la-methode-de-cholesky-by-claude-brezinski.md)

A related algebraic reason for the method's usefulness is that [normal equations](normal-equation.md) involve a [Gram matrix](gram-matrix.md). If a real [matrix](matrix.md) $M$ has [linearly independent](linear-independence.md) columns, then

$$
v^TM^TMv=\|Mv\|_2^2>0\qquad(v\ne0),
$$

so $M^TM$ is a [positive-definite matrix](positive-definite-matrix.md). That gives the structure needed by a [Cholesky decomposition](cholesky-decomposition.md). The historical adjustment problem instead produces $MM^T$ from independent constraint rows; the same argument applies to its [transpose](transpose.md). In numerical least squares, explicitly forming [normal equations](normal-equation.md) squares the [condition number](condition-number.md) of a full-column-rank design [matrix](matrix.md); a [QR decomposition](qr-decomposition.md) can therefore be preferable for accuracy. Indeed, the extreme [singular values](singular-value.md) give $\kappa_2(M^TM)=\sigma_{\max}(M)^2/\sigma_{\min}(M)^2=\kappa_2(M)^2$. The factorization remains useful when a [positive-definite matrix](positive-definite-matrix.md) is already the natural input.

## ↑ Ancestors (9)

1. [Cholesky decomposition](cholesky-decomposition.md)
2. [Positive-definite matrix](positive-definite-matrix.md)
3. [Definite matrix](definite-matrix.md)
4. [Quadratic form](quadratic-form-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
