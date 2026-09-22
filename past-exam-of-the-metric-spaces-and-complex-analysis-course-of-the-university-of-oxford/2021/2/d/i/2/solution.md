<h1 id="2/d/i/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume condition (2). Fix $a\in X$ and $\varepsilon>0$. The [superlevel set](../../../../../../superlevel-set.md)

$$
F=\{x:f(x)\geq f(a)+\varepsilon\}
$$

is a [closed set](../../../../../../closed-set.md) and does not contain $a$. Its [complement](../../../../../../complement-of-a-set.md) is therefore an [open](../../../../../../open-set.md) [neighbourhood](../../../../../../neighbourhood-mathematics.md) of $a$, so some [open ball](../../../../../../open-ball.md) $B(a,r)$ avoids $F$. Consequently $f(x)<f(a)+\varepsilon$ throughout that ball, giving

$$
M_a(r)\leq f(a)+\varepsilon.
$$

The same bound holds for every smaller radius. Taking $r\downarrow0$ and then $\varepsilon\downarrow0$ yields

$$
\boxed{\lim_{r\downarrow0}\sup_{x\in B(a,r)}f(x)\leq f(a).}
$$

Together with the previous implication this proves the equivalence. A [supremum](../../../../../../supremum.md) may equal $f(a)+\varepsilon$ even when every individual value is strictly smaller; the non-strict estimate here handles that possibility.

## ↑ Ancestors (14)

1. [2](../2.md)
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
