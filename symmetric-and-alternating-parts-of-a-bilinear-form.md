# Symmetric and alternating parts of a bilinear form

↑ **Parent:** [Bilinear form](bilinear-form-split.md)

Over a [field](field.md) whose [characteristic](characteristic-of-a-field.md) is not two, a [bilinear form](bilinear-form-split.md) has a unique decomposition into a [symmetric bilinear form](symmetric-bilinear-form.md) $S$ and an [alternating bilinear form](alternating-bilinear-form.md) $K$:

$$
S(v,w)=\frac{B(v,w)+B(w,v)}2,\qquad K(v,w)=\frac{B(v,w)-B(w,v)}2.
$$

Adding and subtracting the equations $B(v,w)=S(v,w)+K(v,w)$ and $B(w,v)=S(v,w)-K(v,w)$ both proves uniqueness and gives these formulas. In [matrix](matrix.md) notation, $S$ has [matrix](matrix.md) $(A+A^T)/2$ and $K$ has [skew-symmetric matrix](skew-symmetric-matrix.md) $(A-A^T)/2$.[Theorem 1.7: symmetric and alternating decomposition](bilinear-forms-by-keith-conrad.md)

The diagonal values $q(v)=B(v,v)$ alone do not determine a general [bilinear form](bilinear-form-split.md), because $K(v,v)=0$ for every [vector](vector.md). For the [matrix of a bilinear form](matrix-of-a-bilinear-form.md) in the example above,

$$
A=\underbrace{\begin{pmatrix}1&1\\1&1\end{pmatrix}}_{\text{symmetric part}}+\underbrace{\begin{pmatrix}0&1\\-1&0\end{pmatrix}}_{\text{alternating part}},\qquad q(x,y)=(x+y)^2.
$$

Thus two different [bilinear forms](bilinear-form-split.md), represented by $A$ and its [symmetric matrix](symmetric-matrix.md) part, have exactly the same [quadratic form](quadratic-form-split.md). To recover a [bilinear form](bilinear-form-split.md) from its diagonal, one needs extra information such as the hypothesis that it is a [symmetric bilinear form](symmetric-bilinear-form.md).

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Coercive bilinear form](coercive-bilinear-form.md)
