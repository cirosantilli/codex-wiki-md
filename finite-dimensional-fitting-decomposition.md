# Finite-dimensional Fitting decomposition

↑ **Parent:** [Fitting lemma](fitting-lemma.md)

Every [linear endomorphism](linear-endomorphism.md) of a finite-dimensional [vector space](vector-space-split.md) admits the displayed [direct sum of vector spaces](direct-sum.md). It separates the part on which repeated application is invertible from the part eventually sent to zero.

**Proof.** [Stabilization of images of powers of a linear map](stabilization-of-images-of-powers-of-a-linear-map.md) gives $\operatorname{im}h^n=\operatorname{im}h^{2n}$. The [rank-nullity theorem](rank-nullity-theorem.md) and nested [null spaces](kernel-of-a-linear-map-split.md) give $\ker h^n=\ker h^{2n}$. If $v=h^nu$ also satisfies $h^nv=0$, then $u\in\ker h^{2n}=\ker h^n$, so $v=0$. Thus the displayed summands have zero [intersection](set-intersection.md). Their [dimensions](dimension-vector-space.md) sum to $n$ by the [rank-nullity theorem](rank-nullity-theorem.md), proving the decomposition.

Both summands are preserved by $h$. On $\operatorname{im}h^n$, stabilization makes $h$ a [surjective linear map](surjective-linear-map.md), hence invertible in finite [dimension](dimension-vector-space.md). On $\ker h^n$, its $n$th power is zero, so the restriction is a [nilpotent linear map](nilpotent-linear-map.md).

## ↑ Ancestors (7)

1. [Fitting lemma](fitting-lemma.md)
2. [Module theory](module-theory-split.md)
3. [Commutative algebra](commutative-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cartan subalgebra existence from a minimal Engel subalgebra](cartan-subalgebra-existence-from-a-minimal-engel-subalgebra.md)
- [Solution](past-exam-of-the-lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford/2007/a/2/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/5/e/solution.md)
- [Stabilization of images of powers of a linear map](stabilization-of-images-of-powers-of-a-linear-map.md)
