# Nondegenerate bilinear form

↑ **Parent:** [Bilinear form](bilinear-form-split.md)

A [bilinear form](bilinear-form-split.md) $B$ is nondegenerate when its [left radical](left-radical-of-a-bilinear-form.md) and [right radical](right-radical-of-a-bilinear-form.md) are both zero: every nonzero [vector](vector.md) can be detected by some pairing, whichever input slot it occupies. On a [finite-dimensional vector space](finite-dimensional-vector-space.md), either condition implies the other, and the following tests are equivalent:

$$
\begin{aligned}
B(v,w)=0\text{ for every }v&\quad\Longrightarrow\quad w=0,\\
V\longrightarrow V^*,\quad w\longmapsto B(-,w)&\quad\text{is an isomorphism},\\
\det A&\ne0.
\end{aligned}
$$

Here $A$ is the [matrix of a bilinear form](matrix-of-a-bilinear-form.md), and $V^*$ is the [dual space](dual-space-split.md). The [linear map](linear-map.md) $w\mapsto B(-,w)$ has [matrix](matrix.md) $A$ in the chosen [basis](basis.md) and its [dual basis](dual-basis.md), so its [kernel](kernel-of-a-linear-map-split.md) is the [right radical](right-radical-of-a-bilinear-form.md). The map $v\mapsto B(v,-)$ has [matrix](matrix.md) $A^T$. An [invertible matrix](invertible-matrix.md) has zero [kernel](kernel-of-a-linear-map-split.md) on both sides, proving the finite-dimensional equivalence. In infinite dimensions, zero [left radical](left-radical-of-a-bilinear-form.md) and [right radical](right-radical-of-a-bilinear-form.md) imply these maps are [injective](injective-function.md), but do not generally make them [surjective](surjective-function.md).[§2: the two maps to the dual space](bilinear-forms-by-keith-conrad.md)

For the real [symmetric bilinear form](symmetric-bilinear-form.md) $B((x,y),(s,t))=xs-yt$, the [determinant](determinant.md) is $-1$. Its [isotropic vector](isotropic-vector.md) $(1,1)$ has zero self-pairing but pairs to $1$ with $(1,0)$, so it is detected. The [alternating bilinear form](alternating-bilinear-form.md) with [matrix](matrix.md) $J$ has [determinant](determinant.md) $1$ and detects every nonzero [vector](vector.md) even though all self-pairings vanish. Neither zero self-pairings nor the absence of [positive definiteness](positive-definiteness.md) implies degeneracy.

Nondegeneracy is useful because it turns a [linear functional](linear-functional.md) into a unique [vector](vector.md). For $A=\operatorname{diag}(1,-1)$, the [linear functional](linear-functional.md) $\ell(s,t)=2s+3t$ is $B((2,-3),(s,t))$; solving for that representing [vector](vector.md) amounts to solving an invertible [system of linear equations](system-of-linear-equations.md). The analogous identification underlies [bilinear orthogonal complements](orthogonal-complement-for-a-bilinear-form.md) and the [dual isomorphisms induced by a nondegenerate pairing](dual-isomorphisms-induced-by-a-nondegenerate-pairing.md).

**Table of contents**

- [Dual isomorphisms induced by a nondegenerate pairing](dual-isomorphisms-induced-by-a-nondegenerate-pairing.md)
- [Symplectic vector space](symplectic-vector-space.md)
  - [Symplectic linear map](symplectic-linear-map.md)
  - [Symplectic subspace](symplectic-subspace.md)
    - [Orientation criterion for a graph of symplectic planes](orientation-criterion-for-a-graph-of-symplectic-planes.md)
  - [Eigenspaces of a symplectic involution](eigenspaces-of-a-symplectic-involution.md)
  - [Symplectic orthogonal complement](symplectic-orthogonal-complement.md)
  - [Isotropic subspace of a symplectic vector space](isotropic-subspace-of-a-symplectic-vector-space.md)
  - [Symplectic basis](symplectic-basis.md)
    - [Paired coordinates of a symplectic basis](paired-coordinates-of-a-symplectic-basis.md)
    - [Four-dimensional symplectic basis change](four-dimensional-symplectic-basis-change.md)
    - [Symplectic Gram-Schmidt process](symplectic-gram-schmidt-process.md)
- [Representation of a bilinear form relative to a nondegenerate bilinear form](representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form.md)

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (44)

- [Bilinear form](bilinear-form-split.md)
- [Cartan criterion for semisimplicity](cartan-criterion-for-semisimplicity.md)
- [Clifford algebra bundle](clifford-algebra-bundle.md)
- [Diamond Lie algebra](diamond-lie-algebra.md)
- [Eigenspaces of a symplectic involution](eigenspaces-of-a-symplectic-involution.md)
- [Invariant bilinear form as an intertwiner](invariant-bilinear-form-as-an-intertwiner.md)
- [Invariant gauge kinetic form](invariant-gauge-kinetic-form.md)
- [Lorentzian manifold](lorentzian-manifold.md)
- [Metric tensor](metric-tensor.md)
- [Minkowski metric](minkowski-metric.md)
- [Nondegeneracy of the trace form of a number field](nondegeneracy-of-the-trace-form-of-a-number-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3/1/iii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-45/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-20/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-20/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-102/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-102/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/12i/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/20h/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-4/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2/19j/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-111/2/d/solution.md)
- [Perfect pairing](perfect-pairing.md)
- [Pseudo-Riemannian manifold](pseudo-riemannian-manifold.md)
- [Representation of a bilinear form relative to a nondegenerate bilinear form](representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form.md)
- [Symplectic basis](symplectic-basis.md)
- [Symplectic Gram-Schmidt process](symplectic-gram-schmidt-process.md)
- [Symplectic linear map](symplectic-linear-map.md)
- [Symplectic manifold](symplectic-manifold.md)
- [Symplectic orthogonal complement](symplectic-orthogonal-complement.md)
- [Symplectic vector space](symplectic-vector-space.md)
- [Totally isotropic subspace](totally-isotropic-subspace.md)
- [Trace-generated maximal-period linear-feedback sequence](trace-generated-maximal-period-linear-feedback-sequence.md)
