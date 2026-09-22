<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $a=\pi^2(\varepsilon^{-1}-1)$. From the supplied [second moment of a mixture likelihood ratio](../../../../../../second-moment-of-a-mixture-likelihood-ratio.md), dropping a nonpositive term gives

$$
\chi^2(P_1\Vert P_0)\leq\frac{(1+a)^n}{d}\leq\frac{e^{na}}d\leq16\nu^2.
$$

The last step uses the assumed separation. It has a real square root only when $16\nu^2d\geq1$; otherwise no parameters satisfy it. The [chi-squared testing lower bound](../../../../../../chi-squared-testing-lower-bound.md) follows from the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md): $\|P_1-P_0\|_{\mathrm{TV}}\leq\frac12\sqrt{\chi^2(P_1\Vert P_0)}\leq2\nu$. Every [statistical hypothesis testing](../../../../../../statistical-hypothesis-test.md) rule has sum of its [Type I error](../../../../../../type-i-and-type-ii-errors.md) and [Type II error](../../../../../../type-i-and-type-ii-errors.md) at least $1-\|P_1-P_0\|_{\mathrm{TV}}$. Its larger error is at least half the sum, hence

$$
\boxed{\inf_\psi\max\{P_0(\psi=1),P_1(\psi=0)\}\geq\tfrac12-\nu.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
