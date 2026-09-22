<h1 id="o/o4/solution">Solution</h1>

↑ **Parent:** [O4](../o4.md)

Let $f_0,f_1$ be densities or probability mass functions relative to a common measure, describing two simple hypotheses. A randomized [hypothesis test](../../../../statistical-hypothesis-test-split.md) is a measurable function $0\leq\varphi\leq1$, whose value is the conditional rejection probability. Fix $0<\alpha<1$. The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) states that a test $\varphi_*$ with $\mathbb E_0\varphi_*=\alpha$ is most powerful among tests with size at most $\alpha$ if it rejects where $f_1>cf_0$, accepts where $f_1<cf_0$, and randomizes as necessary on equality, for a threshold $c\geq0$. Sets where $f_0=0<f_1$ are included in rejection. A [likelihood](../../../../likelihood-function.md)-ratio quantile and boundary randomization supply such a test.

To prove optimality, let $\varphi$ be any competitor with $\mathbb E_0\varphi\leq\alpha$. Pointwise, the threshold rule makes

$$
(\varphi_*-\varphi)(f_1-cf_0)\geq0.
$$

Integrating and rearranging gives

$$
\mathbb E_1\varphi_*-\mathbb E_1\varphi
\geq c(\mathbb E_0\varphi_*-\mathbb E_0\varphi)\geq0.
$$

Thus no competitor of the permitted size has larger [statistical power](../../../../statistical-power.md), proving the lemma. Randomization permits exact size when discrete observations cannot supply it with a deterministic rejection region.

## ↑ Ancestors (12)

1. [O4](../o4.md)
2. [O](../../o.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
