<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The necessary and sufficient condition is

$$
\boxed{\ker T=\{0\}.}
$$

For necessity, if $ST=\operatorname{id}_V$ and $v\in\ker T$, then $v=S(Tv)=S(0)=0$.

For sufficiency, let $e_1,e_2$ be a [basis](../../../../../../../basis.md) of $V$ and suppose the [kernel of a linear map](../../../../../../../kernel-of-a-linear-map-split.md) is trivial. The [vectors](../../../../../../../vector.md) $Te_1,Te_2$ are [linearly independent](../../../../../../../linear-independence.md), since $aTe_1+bTe_2=0$ implies $ae_1+be_2\in\ker T$. Extend them to a [basis](../../../../../../../basis.md) $Te_1,Te_2,w_3$ of $W$. Define a [linear map](../../../../../../../linear-map.md) $S$ by

$$
S(Te_1)=e_1,\qquad S(Te_2)=e_2,\qquad S(w_3)=0.
$$

Then $ST$ agrees with the [identity operator](../../../../../../../identity-operator.md) on a [basis](../../../../../../../basis.md), hence on all of $V$. Thus a [left inverse](../../../../../../../left-inverse.md) exists precisely when $T$ is [injective](../../../../../../../injective-function.md); this is the [linear left inverse criterion](../../../../../../../linear-left-inverse-criterion.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
