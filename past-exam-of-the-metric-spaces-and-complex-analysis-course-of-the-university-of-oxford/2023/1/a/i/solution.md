<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

A [metric space](../../../../../metric-space.md) $(X,d)$ is a [bounded set](../../../../../bounded-set.md) if there is a finite constant $M\geq0$ such that

$$
\boxed{d(x,y)\leq M\quad\text{for every }x,y\in X}.
$$

For nonempty $X$, this is equivalent to containment in an [open ball](../../../../../open-ball.md) of finite radius: the [triangle inequality](../../../../../triangle-inequality.md) converts a radius bound into a diameter bound, and conversely a diameter bound gives a ball of any slightly larger radius about a chosen point.

It is a [complete metric space](../../../../../complete-metric-space.md) if every [Cauchy sequence](../../../../../cauchy-sequence.md) in $X$ has a [limit of a sequence](../../../../../limit-of-a-sequence.md) belonging to $X$. Explicitly, the hypothesis on $(x_n)$ is

$$
\forall\epsilon>0\ \exists N\ \forall m,n\geq N:\ d(x_m,x_n)<\epsilon,
$$

and [completeness](../../../../../completeness.md) requires an $x\in X$ with $d(x_n,x)\to0$. Thus

$$
\boxed{\text{every Cauchy sequence converges in }X}.
$$

Boundedness controls distances; [completeness](../../../../../completeness.md) ensures that these limiting points remain in the space.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
