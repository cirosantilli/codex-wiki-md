<h1 id="a/1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppose for contradiction that $p_n=(u_n,v_n)\in Y$ converges to the origin in the [initial topology](../../../../../initial-topology.md). The [coordinate projections](../../../../../projection-map.md) then give $u_n\to0$ and $v_n\to0$ in the usual [real line](../../../../../real-line.md). [Rectangular bumps detecting nonconvergence](../../../../../rectangular-bumps-detecting-nonconvergence.md), using anisotropic supports, avoids any unsupported regularity assertion about a radial maximum. [Set](../../../../../set-split.md)

$$
\phi(t)=\max(1-|t|,0),\qquad r_n=|u_n|/4,\quad s_n=|v_n|/4,
$$



$$
b_n(x,y)=\phi\!\left(\frac{x-u_n}{r_n}\right)\phi\!\left(\frac{y-v_n}{s_n}\right),\qquad B(x,y)=\sup_n b_n(x,y).
$$

The radii are positive since neither coordinate of $p_n$ vanishes. Each rectangular support misses both coordinate axes, so $B$ vanishes on those axes. For a fixed $y=c\ne0$, all but finitely many vertical support intervals miss $c$, because their centres and radii tend to zero. Hence $B(x,c)$ is a [finite maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) of [continuous functions](../../../../../continuous-function.md) of $x$, and is [continuous](../../../../../continuous-function.md). At $c=0$ it is identically zero. The same argument with the coordinates exchanged proves [separate continuity](../../../../../separate-continuity.md) everywhere. Thus $B$ is [continuous](../../../../../continuous-function.md) for the [initial topology](../../../../../initial-topology.md).

However $B(p_n)=1$ for every $n$, whereas $B(0,0)=0$. This contradicts preservation of [convergent sequences](../../../../../convergent-sequence.md) by a [continuous function](../../../../../continuous-function.md). Therefore **no [sequence](../../../../../sequence.md) from $Y$ converges to the origin**.

The radial hint in the scan is not [separately continuous](../../../../../separate-continuity.md) for every candidate [sequence](../../../../../sequence.md): for $p_n=(2^{-n},2^{-2n})$, its value at the origin is zero, while its value at $(2^{-n},0)$ is at least $1-2(2^{-2n})/\sqrt{2^{-2n}+2^{-4n}}$, which tends to one. The rectangular construction supplies the needed valid proof independently of that hint.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
