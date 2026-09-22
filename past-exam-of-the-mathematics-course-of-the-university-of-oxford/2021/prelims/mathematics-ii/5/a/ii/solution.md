<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n=1$, choose $x=0$, $y=1$. For $n\geq2$, define the [continuous function](../../../../../../../continuous-function.md)

$$
g(t)=f(t+1/n)-f(t),\qquad 0\leq t\leq1-1/n.
$$

Its values at the grid points have the [telescoping sum](../../../../../../../telescoping-sum.md)

$$
\sum_{k=0}^{n-1}g(k/n)=\sum_{k=0}^{n-1}\bigl(f((k+1)/n)-f(k/n)\bigr)=f(1)-f(0)=0.
$$

If one summand is zero, we already have a zero of $g$. Otherwise the summands cannot all have the same sign, so two of these values have opposite signs. The [intermediate value theorem](../../../../../../../intermediate-value-theorem.md) between their arguments gives $t\in[0,1-1/n]$ with $g(t)=0$. Set $x=t$, $y=t+1/n$. Then

$$
\boxed{|x-y|=1/n,\qquad f(x)=f(y).}
$$

This is the [horizontal chord of reciprocal-integer length](../../../../../../../horizontal-chord-of-reciprocal-integer-length.md) property; the [telescoping sum](../../../../../../../telescoping-sum.md) explains why reciprocal [integers](../../../../../../../integer-split.md) appear.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
