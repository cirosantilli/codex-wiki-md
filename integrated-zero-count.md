# Integrated zero count

↑ **Parent:** [Radial zero-counting function](radial-zero-counting-function.md)

Under the hypotheses of [Jensen's formula](jensen-s-formula.md), $f(0)\ne0$ ensures that the [radial zero-counting function](radial-zero-counting-function.md) vanishes for sufficiently small positive $t$. Integrating each zero's contribution separately gives

$$
N_f(R)=\int_0^R\frac{n_f(t)}{t}\,dt
=\sum_{|a|<R}\operatorname{ord}_a f\int_{|a|}^{R}\frac{dt}{t}
=\sum_{|a|<R}\operatorname{ord}_a f\log\frac{R}{|a|}
=L_f(R)-\log|f(0)|.
$$

The values of $n_f$ at its finitely many jump points do not change the [integral](integral-split.md). For $0<r<R$, every zero in the smaller [open disc](open-disc.md) supplies at least $\log(R/r)$ per unit of [multiplicity of a zero](multiplicity-of-a-zero.md), so

$$
n_f(r)\log(R/r)\le N_f(R)\le\log M_f(R)-\log|f(0)|,
\qquad M_f(R)=\max_{|z|=R}|f(z)|.
$$

The second inequality bounds the [circle log-mean of a holomorphic function](circle-log-mean-of-a-holomorphic-function.md) by the [logarithm](logarithm.md) of the largest boundary [complex modulus](complex-modulus.md), recovering the [Jensen zero-count bound](jensen-zero-count-bound.md). An upper bound on boundary growth and a fixed nonzero centre value therefore constrain interior zeros. The factor $\log(R/r)$ also explains why the same estimate becomes weaker as the smaller radius approaches the boundary.

## ↑ Ancestors (8)

1. [Radial zero-counting function](radial-zero-counting-function.md)
2. [Jensen's formula](jensen-s-formula.md)
3. [Holomorphic function](holomorphic-function-split.md)
4. [Complex analysis](complex-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Jensen's formula](jensen-s-formula.md)
