<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Ehrenfeucht theory of an increasing named sequence](../../../../../../ehrenfeucht-theory-of-an-increasing-named-sequence.md) is complete and has [quantifier elimination](../../../../../../quantifier-elimination.md): the usual one-point cut argument for [dense linear orders without endpoints](../../../../../../dense-linear-order-without-endpoints.md) works with the finitely many constants occurring in a formula. Complete types are consequently determined by order relations to the named constants and to any additional parameters.

In the model where the sequence is unbounded above, every finite tuple lies below some $c_N$. Its order relations to $c_0,\ldots,c_N$, together with its internal equality and order pattern, determine its relations to every later constant as well. This finite condition isolates its [complete type](../../../../../../complete-type.md). Thus model (ii) is an [atomic model](../../../../../../atomic-model.md). It is not omega-saturated, because the finitely satisfiable type $\{c_i<x:i\in\mathbb N\}$ has no realization.

In either bounded model, a point above every $c_i$ realizes the type

$$
p_\infty(x)=\{c_i<x:i\in\mathbb N\}.
$$

This type is not isolated. Any formula belonging to it uses only finitely many constants after [quantifier elimination](../../../../../../quantifier-elimination.md), and its order condition can also be realized below a sufficiently late $c_j$. That realization fails one of the later inequalities in $p_\infty$. Hence neither bounded model is atomic.

In model (i), let $d$ be the least upper bound. The type $\{c_i<x:i\in\mathbb N\}\cup\{x<d\}$ over the single parameter $d$ is finitely satisfiable by density but unrealized, so this model is not omega-saturated.

In model (iii), the upper tail $U=\{x:c_i<x\text{ for all }i\}$ has no least element. Every consistent one-type over finitely many parameters is realizable. Indeed, it is either an equality type, a cut below or between some of the named constants, or a cut in $U$. The first two cases are realized by equality or by density in the relevant interval. In $U$, finitely many parameters divide the tail into finitely many intervals, each relevant nonempty interval having points by density, absence of a least element in $U$, and absence of a last element in the order. This realizes the third case too. There is no other cut among the increasing sequence: a proper initial segment of its indices is finite. Successive one-variable realizations give all finite-tuple types. Therefore

$$
\boxed{\text{Atomic: (ii) only.}\qquad\text{Omega-saturated: (iii) only.}}
$$

A least upper bound is thus precisely the obstruction to filling the additional finite-parameter cut in model (i).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
