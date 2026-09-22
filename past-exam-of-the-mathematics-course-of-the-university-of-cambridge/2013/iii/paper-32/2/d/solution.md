<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For equal independent samples, take $p_B=0.0002$, $p_C=0.0006$ and $\bar p=0.0004$ in the two-proportion formula, with two-sided $\alpha=0.05$ and power $1-\beta=0.80$. It gives

$$
n\simeq\frac{\left[1.95996\sqrt{2(0.0004)(0.9996)}
+0.84162\sqrt{0.0002(0.9998)+0.0006(0.9994)}\right]^2}
{(0.0004)^2}
=39227.52.
$$

Thus the usual normal planning estimate is

$$
\boxed{\text{about }3.92\text{ blocks of 10,000 per supplier,
or }4\text{ whole blocks each}.}
$$

The combined approximate design therefore checks about eight blocks, with about eight positive batches from B and twenty-four from C at the rounded design.

Those expected counts are low enough for test discreteness to matter. If a genuinely exact two-sided [Fisher exact test](../../../../../../fisher-s-exact-test.md) is specified, the null allocation of the positive batches between two equal-size suppliers is [hypergeometric](../../../../../../hypergeometric-distribution.md), conditional on their total. Under the proposed alternative, its power is obtained by summing the independent binomial [probabilities](../../../../../../probability.md) over the exact rejection region:

$$
\operatorname{Power}(n)=\sum_{b,c:\,p_F(b,c)\leq0.05}
\Pr\{\operatorname{Bin}(n,0.0002)=b\}
\Pr\{\operatorname{Bin}(n,0.0006)=c\}.
$$

An independent calculation of the [exact power of Fisher's exact test](../../../../../../exact-power-of-fisher-s-exact-test.md) gives about $0.7750$ at $n=40000$ and $0.8728$ at $n=50000$. Consequently **five whole 10,000-batch blocks per supplier suffice for at least 80% power with this conservative exact test**. Four blocks are the intended normal-approximation answer, not an exact 80% guarantee irrespective of the chosen test. The distinction is a property of rare-event discreteness, not a change in the proposed effect size.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
