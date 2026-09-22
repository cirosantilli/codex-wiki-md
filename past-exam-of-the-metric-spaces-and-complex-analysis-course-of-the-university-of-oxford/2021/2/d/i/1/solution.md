<h1 id="2/d/i/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume condition (1). For fixed $a$, the [supremum](../../../../../../supremum.md)

$$
M_a(r)=\sup_{x\in B(a,r)}f(x)
$$

is nondecreasing as $r$ increases. Therefore its limit as $r\downarrow0$ exists in the extended [real numbers](../../../../../../real-number.md) and equals $\inf_{r>0}M_a(r)$. Because $a\in B(a,r)$, it is at least $f(a)$. Condition (1) says precisely that this limit is $f(a)$.

It follows that for every $\varepsilon>0$ there is $r>0$ with $M_a(r)<f(a)+\varepsilon$. Fix $C\in\mathbb R$ and $a$ with $f(a)<C$. Taking $\varepsilon=C-f(a)$ produces an [open ball](../../../../../../open-ball.md) on which $f(x)<C$. Thus $\{x:f(x)<C\}$ is an [open set](../../../../../../open-set.md), and its [complement](../../../../../../complement-of-a-set.md)

$$
\boxed{\{x:f(x)\geq C\}\text{ is a closed set}.}
$$

This proves (1) implies (2). The property being characterized is [upper semicontinuity](../../../../../../upper-semicontinuity.md).

## ↑ Ancestors (14)

1. [1](../1.md)
2. [i](../../i.md)
3. [d](../../../d.md)
4. [2](../../../../2.md)
5. [2021](../../../../../2021-split.md)
6. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../../split.md)
7. [Metric spaces and complex analysis course of the University of Oxford](../../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
