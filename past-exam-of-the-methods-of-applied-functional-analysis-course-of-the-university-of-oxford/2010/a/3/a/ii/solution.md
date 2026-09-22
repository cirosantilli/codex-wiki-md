<h1 id="a/3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Introduce coordinates $s=x+y$, $t=x-y$, so $dx\,dy=\tfrac12ds\,dt$. For a [test function](../../../../../../test-function.md) $\varphi(x,y)=\Phi(s,t)$,

$$
V\cdot\nabla\varphi=\mathbf1_{s>0}(\Phi_s+\Phi_t)+\mathbf1_{s<0}(\Phi_s-\Phi_t)=\Phi_s+\operatorname{sgn}(s)\Phi_t
$$

[almost everywhere](../../../../../../almost-everywhere.md). Hence

$$
\int_{\mathbb R^2}V\cdot\nabla\varphi=\frac12\int_{\mathbb R^2}\bigl(\Phi_s+\operatorname{sgn}(s)\Phi_t\bigr)\,ds\,dt=0.
$$

The first derivative integrates to zero in $s$, and the second to zero in $t$, using compact support. Thus $\boxed{\operatorname{div}V=0}$ as a [weak divergence](../../../../../../weak-divergence.md). Geometrically, the jump across $x+y=0$ is $(1,-1)$, perpendicular to its normal $(1,1)$; there is no distributional flux concentrated on the interface.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
