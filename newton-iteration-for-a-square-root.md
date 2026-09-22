# Newton iteration for a square root

↑ **Parent:** [Newton's method in optimization](newton-s-method-in-optimization.md)

For $c>0$ and $a_0>0$, the displayed [recurrence relation](recurrence-relation.md) stays positive and satisfies

$$
a_{n+1}^2-c=\frac{(a_n^2-c)^2}{4a_n^2}\geq0.
$$

After the first step, $a_n^2\geq c$, so $a_{n+1}-a_n=(c-a_n^2)/(2a_n)\leq0$. The [bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md) gives a [limit of a sequence](limit-of-a-sequence.md) $L\geq0$; the inequality $L^2\geq c>0$ makes $L$ positive, and passage to the [limit of a sequence](limit-of-a-sequence.md) in the [recurrence relation](recurrence-relation.md) gives $L^2=c$. This proves existence of the positive [square root](square-root.md) without assuming it in the construction. Once $s=\sqrt c$ is known, the exact error identity $a_{n+1}-s=(a_n-s)^2/(2a_n)$ explains the eventual [quadratic convergence](quadratic-convergence.md).

**Table of contents**

- [Negative-parameter square-root iteration changes sign infinitely often](negative-parameter-square-root-iteration-changes-sign-infinitely-often.md)

## ↑ Ancestors (5)

1. [Newton's method in optimization](newton-s-method-in-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-ii/2/b/ii/solution.md)
