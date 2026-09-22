<h1 id="1/1/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A finite-valued [global minimizer](../../../../../../../../global-minimizer.md) of the [functional](../../../../../../../../functional.md) $E$ is an element $\bar u\in\operatorname{dom}E$ satisfying

$$
\boxed{E(\bar u)=\inf_{u\in\mathcal U}E(u)<+\infty,\qquad
\operatorname{dom}E=\{u:E(u)<+\infty\}.}
$$

Here $\operatorname{dom}E$ is its [effective domain](../../../../../../../../effective-domain.md). The finite-value convention avoids treating an infeasible problem as solved.

The [functional](../../../../../../../../functional.md) is a [proper extended-real function](../../../../../../../../proper-extended-real-function.md) if its [effective domain](../../../../../../../../effective-domain.md) is nonempty; the specified codomain already excludes $-\infty$. It has [coercivity](../../../../../../../../coercive-function.md) if $\|u_n\|\to\infty$ always implies $E(u_n)\to+\infty$, equivalently every finite [sublevel set](../../../../../../../../sublevel-set.md) is bounded. It is $\tau$-[sequentially lower semicontinuous](../../../../../../../../sequential-lower-semicontinuity.md) if

$$
\boxed{u_n\xrightarrow{\tau}u\ \Longrightarrow\
E(u)\leq\liminf_{n\to\infty}E(u_n).}
$$

The topology in this definition matters: norm [sequential lower semicontinuity](../../../../../../../../sequential-lower-semicontinuity.md) and weak [sequential lower semicontinuity](../../../../../../../../sequential-lower-semicontinuity.md) need not coincide for a nonconvex [functional](../../../../../../../../functional.md).

## ↑ Ancestors (13)

1. [A](../a.md)
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
