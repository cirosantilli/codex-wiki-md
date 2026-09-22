<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The tensor denoted $X\otimes df$ acts as the rank-one [endomorphism](../../../../../../endomorphism.md) $Y\mapsto df(Y)X=Y(f)X$. In the paper's covector-first ordering it is written $df\otimes X$, using the canonical interchange of tensor factors; this is the same [endomorphism](../../../../../../endomorphism.md).

On any [smooth function](../../../../../../smooth-function.md) $h$,

$$
(f\mathcal L_X-\mathcal L_{fX})h=fX(h)-(fX)(h)=0.
$$

On a [vector field](../../../../../../vector-field.md) $Y$, the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) gives

$$
[fX,Y]=f[X,Y]-Y(f)X,
$$

so

$$
(f\mathcal L_X-\mathcal L_{fX})Y=Y(f)X=D_{X\otimes df}Y.
$$

Multiplication by $f$ preserves the tensor-product [Leibniz rule](../../../../../../leibniz-rule.md) and commutation with [tensor contractions](../../../../../../tensor-contraction.md), since the latter are linear over [smooth functions](../../../../../../smooth-function.md). Hence the difference is a real-linear contraction-compatible [tensor derivation](../../../../../../tensor-derivation.md) whose scalar operator is zero. Its agreement with $D_{X\otimes df}$ on functions and [vector fields](../../../../../../vector-field.md) determines its action on every tensor by uniqueness:

$$
\boxed{D_{X\otimes df}=f\mathcal L_X-\mathcal L_{fX}.}
$$

For example, on a [differential one-form](../../../../../../one-form.md) this gives $-\omega(X)df$. Equivalently $\mathcal L_{fX}\omega=f\mathcal L_X\omega+\omega(X)df$, which checks the sign independently. This is the [scaled Lie derivative defect identity](../../../../../../scaled-lie-derivative-defect-identity.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
