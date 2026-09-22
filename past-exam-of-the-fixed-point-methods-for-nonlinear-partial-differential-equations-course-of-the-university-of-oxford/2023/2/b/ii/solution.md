<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $P=\{w\in L^2(\Omega):w\geq0\text{ almost everywhere}\}$. For $g\in L^2(\Omega)$, define $Gg=z\in H_0^1(\Omega)$ by

$$
\int_\Omega\nabla z\cdot\nabla v\,dx=\int_\Omega gv\,dx
\qquad(v\in H_0^1(\Omega)).
$$

The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) guarantees a unique $z$: the [bilinear form](../../../../../bilinear-form-split.md) on the left is bounded and [coercive](../../../../../coercive-bilinear-form.md) in the [norm](../../../../../norm.md) $\|\nabla\cdot\|_2$, and the right side is a bounded [linear functional](../../../../../linear-functional.md) by the [Poincaré inequality](../../../../../poincare-inequality.md). Testing with $z$ gives

$$
\|\nabla Gg\|_2\leq C_P\|g\|_2,
\qquad\|Gg\|_2\leq C_P^2\|g\|_2.
$$

Define $T:P\to L^2(\Omega)$ by $Tw=G(1+\sqrt w)$. This actually maps into $P$. Indeed the [weak maximum principle](../../../../../weak-maximum-principle-for-elliptic-operators.md) says that a [weak solution](../../../../../weak-solution.md) $z\in H_0^1(\Omega)$ of $-\Delta z=g\geq0$ is nonnegative [almost everywhere](../../../../../almost-everywhere.md). Here $1+\sqrt w\geq0$ and belongs to $L^2(\Omega)$. Directly, taking the [negative part](../../../../../negative-part-of-a-real-valued-function.md) $z^-=\max\{-z,0\}$ as a [test function](../../../../../test-function.md) gives $-\|\nabla z^-\|_2^2=\int_\Omega gz^-\,dx\geq0$, so $z^-=0$ by the [Poincaré inequality](../../../../../poincare-inequality.md).

The required [fixed point](../../../../../fixed-point.md) formulation is

$$
\boxed{u\in P,\qquad u=Tu=G(1+\sqrt u).}
$$

Every such [fixed point](../../../../../fixed-point.md) belongs automatically to $H_0^1(\Omega)$ and satisfies part (b)(i). Conversely, uniqueness in the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) makes every nonnegative [weak solution](../../../../../weak-solution.md) a [fixed point](../../../../../fixed-point.md) of $T$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
