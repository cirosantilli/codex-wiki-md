<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x<y$, [finite additivity](../../../../finite-additivity-of-a-set-function.md) on the [disjoint](../../../../disjoint-sets.md) pieces of the half-line gives

$$
h(y)-h(x)=m\bigl(E\cap(x,y]\bigr).
$$

By [monotonicity of a measure](../../../../monotonicity-of-a-measure.md) and the [Lebesgue measure](../../../../lebesgue-measure.md) of an [interval](../../../../interval-mathematics.md),

$$
0\leq h(y)-h(x)\leq m((x,y])=y-x.
$$

Exchanging the two points if necessary proves

$$
\boxed{|h(y)-h(x)|\leq|y-x|\qquad(x,y\in\mathbb R).}
$$

Thus the [cumulative measure of a finite-measure set](../../../../cumulative-measure-of-a-finite-measure-set.md) is a [Lipschitz function](../../../../lipschitz-continuity.md) with [Lipschitz constant](../../../../lipschitz-constant.md) at most one, hence is **[uniformly continuous](../../../../uniform-continuity.md)**: given $\varepsilon>0$, the choice $\delta=\varepsilon$ works simultaneously at every point.

To locate its endpoint [limits](../../../../limit-of-a-function.md), the [measurable sets](../../../../measurable-set.md) $E\cap(-\infty,N]$ increase to $E$, so [continuity from below of a measure](../../../../continuity-from-below-of-a-measure.md) gives $h(N)\to m(E)$. The [measurable sets](../../../../measurable-set.md) $E\cap(-\infty,-N]$ decrease to the [empty set](../../../../empty-set.md) and all have finite [measure](../../../../measure-split.md), so [continuity from above of a measure](../../../../continuity-from-above-of-a-measure.md) gives $h(-N)\to0$. Since $h$ is nondecreasing,

$$
\lim_{x\to-\infty}h(x)=0,\qquad
\lim_{x\to\infty}h(x)=m(E).
$$

For $0<c<m(E)$, choose $R>0$ with $h(-R)<c<h(R)$. The [intermediate value theorem](../../../../intermediate-value-theorem.md) on $[-R,R]$ gives $t$ with $h(t)=c$. Then

$$
\boxed{A=E\cap(-\infty,t]\text{ is Lebesgue measurable and }m(A)=c.}
$$

The endpoint values $c=0,m(E)$ can also be achieved by $A=\varnothing,E$. This proves [divisibility of Lebesgue measure](../../../../divisibility-of-lebesgue-measure.md) for arbitrary finite-measure [Lebesgue measurable sets](../../../../lebesgue-measurable-set.md) on the [real line](../../../../real-line.md), including unbounded ones. The [non-atomic measure](../../../../non-atomic-measure.md) structure permits prescribed fractions of [measure](../../../../measure-split.md); a [measure](../../../../measure-split.md) concentrated at one point would not have this property.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
