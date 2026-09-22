# Positive-definiteness threshold in a two-by-two family

↑ **Parent:** [Positive definiteness](positive-definiteness.md)

Vary the coupling in the opening example. The [eigenvectors](eigenvector.md) $e_+=(1,1)^T/\sqrt2$ and $e_-=(1,-1)^T/\sqrt2$ form a fixed [orthonormal eigenbasis](orthonormal-eigenbasis.md), with [eigenvalues](eigenvalue.md) $3+t$ and $3-t$. Writing a [vector](vector.md) as $ue_++ve_-$ gives

$$
q_t=3x^2+2txy+3y^2=(3+t)u^2+(3-t)v^2.
$$

For $|t|<3$, both directions cost energy and $A_t$ is a [positive-definite matrix](positive-definite-matrix.md). At $t=3$, the [quadratic form](quadratic-form-split.md) is $6u^2$: the entire line spanned by $e_-$ has zero energy, and $A_t$ is a singular [positive semidefinite matrix](positive-semidefinite-matrix.md). At $t=-3$, the flat line is instead spanned by $e_+$. For $|t|>3$, the [quadratic form](quadratic-form-split.md) is an [indefinite quadratic form](indefinite-quadratic-form.md); one direction lowers the energy without bound as its displacement grows. At $t=4$, for instance, $q_t(e_+)=7$ while $q_t(e_-)=-1$.

<a id="image-eigenvalues-and-directional-energies-across-the-positivity-threshold"></a>
![](quadratic-energy-eigenvalue-threshold.png)

**[Figure 4](#image-eigenvalues-and-directional-energies-across-the-positivity-threshold). Eigenvalues and directional energies across the positivity threshold**.

The geometric transition is precise. For $|t|<3$, $q_t=1$ is an [ellipse](ellipse.md). At $t=3$, it consists of the two parallel lines $u=\pm1/\sqrt6$, extending freely in the zero-energy direction. For $t>3$, it is a [hyperbola](hyperbola.md). The boundary case retains nonnegative energy but loses both the bounded positive [level sets](level-set.md) and the unique zero-energy [vector](vector.md).

## ↑ Ancestors (9)

1. [Positive definiteness](positive-definiteness.md)
2. [Positive-definite bilinear form](positive-definite-bilinear-form.md)
3. [Symmetric bilinear form](symmetric-bilinear-form.md)
4. [Bilinear form](bilinear-form-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
