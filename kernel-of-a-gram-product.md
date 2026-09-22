# Kernel of a Gram product

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map-split.md)

For a real [matrix](matrix.md) $T$, a [Gram product](gram-product.md) has the displayed [null space](kernel-of-a-linear-map-split.md). Here [Gram product](gram-product.md) means a product $TT^\top$ or $T^\top T$.

**Proof.** The inclusion from right to left is immediate. Conversely, if $TT^\top x=0$, then

$$
0=x^\top TT^\top x=\|T^\top x\|^2,
$$

so $T^\top x=0$. Similarly $\ker(T^\top T)=\ker T$. Thus these [positive semidefinite matrices](positive-semidefinite-matrix.md) retain the relevant [matrix rank](matrix-rank.md) of $T$. The argument uses the positive [Euclidean norm](euclidean-norm.md); a corresponding statement for an arbitrary indefinite [bilinear form](bilinear-form-split.md) need not hold.

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gram product](gram-product.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/4/g/solution.md)
