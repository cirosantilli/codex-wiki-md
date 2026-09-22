# Bounded bilinear form

↑ **Parent:** [Bilinear form](bilinear-form.md)

A [bilinear form](bilinear-form.md) $B:X\times X\to\mathbb R$ on a real [normed vector space](normed-vector-space.md) is bounded when one constant $0\leq C<\infty$ satisfies

$$
|B(u,v)|\leq C\|u\|\|v\|\qquad(u,v\in X).
$$

This is an upper bound on the magnitude of every pairing. It says nothing about the sign of $B(v,v)$ and does not require a [symmetric bilinear form](symmetric-bilinear-form.md). The chosen [norm](norm.md) is part of the hypothesis. Boundedness is equivalent to joint [continuity](continuous-function.md), as shown by the [boundedness criterion for a bilinear form](boundedness-criterion-for-a-bilinear-form.md).[§2.2, Theorem 2.7(ii): continuity bound](introduction-to-finite-element-methods-by-christian-clason.md)

For example, on $\mathbb R^2$ with the [Euclidean norm](euclidean-norm.md), the [bilinear forms](bilinear-form.md)

$$
B_-(u,v)=u_1v_1-u_2v_2,\qquad B_0(u,v)=u_1v_1
$$

both satisfy the upper bound with $C=1$, by the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Yet their [quadratic forms](quadratic-form.md) are $B_-(v,v)=x^2-y^2$ and $B_0(v,v)=x^2$: the former takes negative values and the latter vanishes at the nonzero [vector](vector.md) $(0,1)$. Thus neither is a [coercive bilinear form](coercive-bilinear-form.md). The latter is also a [degenerate bilinear form](degenerate-bilinear-form.md), whereas $B_-$ is [nondegenerate](nondegenerate-bilinear-form.md). Boundedness controls size, not positivity or loss of directions.

Every [bilinear form](bilinear-form.md) on a real or complex [finite-dimensional vector space](finite-dimensional-vector-space.md) equipped with any [norm](norm.md) is bounded. In [coordinates](coordinate-linear-algebra.md), write $B(u,v)=u^TAv$ using its [matrix of a bilinear form](matrix-of-a-bilinear-form.md). The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $|u^TAv|\leq\|A\|_2\|u\|_2\|v\|_2$, with $\|A\|_2$ the [spectral norm](matrix-2-norm.md); [finite-dimensional equivalence of norms](finite-dimensional-equivalence-of-norms.md) transfers this to the chosen [norm](norm.md). The conclusion concerns each fixed [norm](norm.md) and fixed [bilinear form](bilinear-form.md): it does not supply a single constant for an arbitrary family of [matrices](matrix.md) or changing dimensions.

On an [infinite-dimensional vector space](infinite-dimensional-vector-space.md), the upper bound is an additional condition. Equip the [finitely supported sequences](finitely-supported-sequence.md) $c_{00}$ with the [norm](norm.md) inherited from the [l2 sequence space](l2-sequence-space.md) and set

$$
B(u,v)=\sum_{n\geq1}n u_n v_n.
$$

Each pairing is a finite sum, so this is a well-defined [bilinear form](bilinear-form.md). For the [basis vector](basis-vector.md) $e_n$, however, $\|e_n\|_2=1$ and $B(e_n,e_n)=n$; no finite $C$ works. It is even a [coercive bilinear form](coercive-bilinear-form.md) with $\alpha=1$, since $\sum n v_n^2\geq\sum v_n^2$. Consequently coercivity alone does not imply boundedness on a [normed vector space](normed-vector-space.md). This example uses $c_{00}$, which is not a [Hilbert space](hilbert-space-split.md); it does not define this pairing on all of the [l2 sequence space](l2-sequence-space.md).

A [bounded bilinear form](bounded-bilinear-form.md) defines a [bounded linear operator](continuous-linear-operator.md) $T:X\to X'$ by $(Tu)(v)=B(u,v)$, where $X'$ is the [continuous dual space](continuous-dual-space-split.md). Its [operator norm](operator-norm.md) is the smallest admissible $C$:

$$
\|T\|=\sup_{u\ne0,\,v\ne0}\frac{|B(u,v)|}{\|u\|\|v\|}.
$$

This converts an upper bound for pairings into an upper bound for a [linear map](linear-map.md) taking an unknown [vector](vector.md) to a [linear functional](linear-functional.md).

**Table of contents**

- [Grothendieck inequality](grothendieck-inequality.md)
  - [Grothendieck theorem for L1 to Hilbert operators](grothendieck-theorem-for-l1-to-hilbert-operators.md)
    - [Rademacher span is not complemented in L1](rademacher-span-is-not-complemented-in-l1.md)
- [Boundedness criterion for a bilinear form](boundedness-criterion-for-a-bilinear-form.md)

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Bounded bilinear form](bounded-bilinear-form.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Coercive variable-coefficient Dirichlet form](coercive-variable-coefficient-dirichlet-form.md)
- [Elliptic boundary value problem](elliptic-boundary-value-problem-split.md)
- [Lax-Milgram theorem](lax-milgram-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/23h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/23h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105/2/c/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105/2/e/solution.md)
- [Quadratic functional](quadratic-functional.md)
- [Quadratic variational principle for a symmetric positive operator](quadratic-variational-principle-for-a-symmetric-positive-operator.md)
