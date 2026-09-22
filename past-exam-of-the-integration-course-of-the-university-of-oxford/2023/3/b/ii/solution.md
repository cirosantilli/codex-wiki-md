<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**True.** Replace the dominating representative by $|g|$ if necessary, and take the countable union of the exceptional [Lebesgue null sets](../../../../../lebesgue-null-set.md) so that every bound holds off a single null set. Since the interval has [Lebesgue measure](../../../../../lebesgue-measure.md) one, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\int_0^1|g|^2\,dx\leq\left(\int_0^1|g|^4\,dx\right)^{1/2}\left(\int_0^1 1\,dx\right)^{1/2}<\infty.
$$

Thus $g^2$ is a [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md). The squared functions satisfy $|f_n|^2\to0$ pointwise and $|f_n|^2\leq|g|^2$ [almost everywhere](../../../../../almost-everywhere.md). The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore yields

$$
\boxed{\|f_n\|_2^2=\int_0^1|f_n|^2\,dx\longrightarrow0.}
$$

This uses the [Lp inclusion on a finite measure space](../../../../../lp-inclusion-on-a-finite-measure-space.md) to turn the assumed fourth-power bound into the second-power domination actually needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
