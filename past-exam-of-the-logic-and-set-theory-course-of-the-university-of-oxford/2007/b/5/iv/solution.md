<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Fix $m,n$ and induct on $k$. For $k=0$,

$$
m\cdot(n+0)=m\cdot n=m\cdot n+0=m\cdot n+m\cdot0.
$$

For the induction step, use the [multiplication](../../../../../multiplication.md) [recursion](../../../../../recursion-computer-science.md), the [induction hypothesis](../../../../../induction-hypothesis.md), and [addition](../../../../../addition.md) [associativity](../../../../../associative-property.md) from (i):

$$
\begin{aligned}
m\cdot(n+k^+)&=m\cdot(n+k)^+\\
&=m\cdot(n+k)+m\\
&=(m\cdot n+m\cdot k)+m\\
&=m\cdot n+(m\cdot k+m)\\
&=m\cdot n+m\cdot k^+.
\end{aligned}
$$

Thus

$$
\boxed{m\cdot(n+k)=m\cdot n+m\cdot k.}
$$

This establishes the indicated distributive law without assuming [multiplication](../../../../../multiplication.md) is commutative.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
