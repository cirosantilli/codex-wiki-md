<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Bayes' theorem](../../../../../../../bayes-theorem.md) gives

$$
\log p(\theta\mid y)=\log L(\theta)+\log\pi(\theta)-\log Z.
$$

Taking its posterior expectation after subtracting $\log\pi(\theta)$ yields

$$
D_{\mathrm{KL}}(p(\theta\mid y)\Vert\pi)
=\mathbb E_{\theta\mid y}\log L(\theta)-\log Z.
$$

**Thus the equality holds for every proper prior and valid likelihood for which the displayed expectations are well-defined.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
