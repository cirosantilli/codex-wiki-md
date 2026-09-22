# Kernel stabilization for a normal operator

↑ **Parent:** [Normal operator](normal-operator.md)

For a [normal operator](normal-operator.md) on a real or complex [inner product space](inner-product-space.md), equality of $\|Tv\|$ and $\|T^*v\|$ gives $\ker T=\ker T^*$. If $T^2v=0$, put $w=Tv$. Then $Tw=0$ forces $T^*w=0$, and the [adjoint operator](adjoint-operator.md) identity gives

$$
\|w\|^2=\langle Tv,w\rangle=\langle v,T^*w\rangle=0.
$$

Thus $Tv=0$ and $\ker T^2=\ker T$. Applying this implication successively to $T^{k-2}v,T^{k-3}v,\ldots,v$ proves

$$
\boxed{\ker T^k=\ker T\quad\text{for every integer }k\geq1}.
$$

In particular a [nilpotent](nilpotent.md) [normal operator](normal-operator.md) is zero. The argument uses no [spectral theorem](spectral-theorem.md).

## ↑ Ancestors (9)

1. [Normal operator](normal-operator.md)
2. [Adjoint operator](adjoint-operator.md)
3. [Riesz representation theorem](riesz-representation-theorem.md)
4. [Hilbert space](hilbert-space-split.md)
5. [Functional analysis](functional-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Minimal polynomial of a normal operator](minimal-polynomial-of-a-normal-operator.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/3/b/ii/solution.md)
