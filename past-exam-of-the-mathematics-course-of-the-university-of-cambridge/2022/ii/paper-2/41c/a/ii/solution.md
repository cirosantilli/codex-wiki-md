<h1 id="41c/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Iteration gives

$$
\widehat u^{\,n}(\theta)=H(\theta)^n\widehat u^{\,0}(\theta).
$$

If $|H(\theta)|\leq1$ everywhere, the [Parseval identity](../../../../../../../parseval-identity.md) gives

$$
\|u^n\|_{\ell^2}^2
=\frac1{2\pi}\int_{-\pi}^{\pi}
|H(\theta)|^{2n}|\widehat u^{\,0}(\theta)|^2\,d\theta
\leq\|u^0\|_{\ell^2}^2.
$$

Conversely, if $|H(\theta_0)|>1$, continuity supplies a neighbourhood on which $|H|\geq1+\epsilon$. Choose nonzero square-integrable Fourier data supported there. Its norm then grows at least as $(1+\epsilon)^n$, contradicting boundedness. Hence

$$
\boxed{\{u^n\}\text{ is bounded for every }u^0
\iff |H(\theta)|\leq1\text{ for all }\theta}.
$$

This is the one-step [von Neumann stability analysis](../../../../../../../von-neumann-stability-analysis.md) criterion.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [41C](../../../41c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
