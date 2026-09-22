<h1 id="1/1/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take the [weak topology](../../../../../../../../weak-topology-split.md) on the [reflexive Banach space](../../../../../../../../reflexive-banach-space.md) $\mathcal U$. A [bounded linear operator](../../../../../../../../continuous-linear-operator.md) is weak-to-weak continuous: $u_n\rightharpoonup u$ implies $\langle Ku_n,v\rangle\to\langle Ku,v\rangle$ for every $v\in\mathcal V$, by its [adjoint operator](../../../../../../../../adjoint-operator.md). The [weak lower semicontinuity of the Hilbert norm](../../../../../../../../weak-lower-semicontinuity-of-the-hilbert-norm.md) therefore makes $D(u)=\|Ku-f\|$ weakly [sequentially lower semicontinuous](../../../../../../../../sequential-lower-semicontinuity.md).

This [functional](../../../../../../../../functional.md) is finite everywhere and nonnegative. If it has [coercivity](../../../../../../../../coercive-function.md), the [direct method in the calculus of variations](../../../../../../../../direct-method-in-the-calculus-of-variations.md) supplies a [global minimizer](../../../../../../../../global-minimizer.md) $\bar u$. Squaring the residual does not change its [global minimizers](../../../../../../../../global-minimizer.md). Here the [adjoint operator](../../../../../../../../adjoint-operator.md) has codomain $\mathcal U^*$, since the source is a [Banach space](../../../../../../../../banach-space-split.md). Differentiating the squared residual along every real direction $h\in\mathcal U$ gives $\operatorname{Re}\langle K^*(K\bar u-f),h\rangle=0$ in the [dual pairing](../../../../../../../../dual-pairing.md), hence the [normal equation for a linear inverse problem](../../../../../../../../normal-equation-for-a-linear-inverse-problem.md) $K^*(K\bar u-f)=0$. Hence

$$
\boxed{f=K\bar u+(f-K\bar u)\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

The converse fails. For $K:\mathbb R^2\to\mathbb R$, $K(x,y)=x$, and $f=1$, the datum is in the [operator range](../../../../../../../../range-of-a-bounded-linear-operator.md), but $D(1,n)=0$ while $\|(1,n)\|\to\infty$. Thus **admissible data do not imply [coercivity](../../../../../../../../coercive-function.md) of the residual**; an unpenalized [null space](../../../../../../../../kernel-of-a-linear-map.md) already prevents it.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [1](../../../../1.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2018](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
