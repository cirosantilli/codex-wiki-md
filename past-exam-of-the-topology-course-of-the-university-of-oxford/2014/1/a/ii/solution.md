<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $f$ is [continuous](../../../../../continuous-function.md) and $x\in\overline A$. Every [open neighbourhood](../../../../../open-neighbourhood.md) $V$ of $f(x)$ has an [open](../../../../../open-set.md) [preimage](../../../../../preimage.md) containing $x$, which meets $A$. Hence $V$ meets $f(A)$, proving $f(x)\in\overline{f(A)}$.

Conversely, suppose the indicated inclusion holds for every subset. To prove [continuity](../../../../../continuous-function.md), take any [closed set](../../../../../closed-set.md) $C\subseteq Y$ and put $A=f^{-1}(C)$. Since $f(A)\subseteq C$ and $C$ is [closed](../../../../../closed-set.md),

$$
f(\overline A)\subseteq\overline{f(A)}\subseteq C.
$$

Thus $\overline A\subseteq f^{-1}(C)=A$, so $A$ is [closed](../../../../../closed-set.md). Every [closed set](../../../../../closed-set.md) has [closed](../../../../../closed-set.md) [preimage](../../../../../preimage.md), which is the closed-set characterization of [continuity](../../../../../continuous-function.md).

$$
\boxed{f\text{ continuous}\iff f(\overline A)\subseteq\overline{f(A)}\text{ for every }A\subseteq X.}
$$

This is the [closure characterization of continuity](../../../../../closure-characterization-of-continuity.md); it requires no [Hausdorff](../../../../../hausdorff-space.md) or [metric](../../../../../metric.md) hypothesis.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
