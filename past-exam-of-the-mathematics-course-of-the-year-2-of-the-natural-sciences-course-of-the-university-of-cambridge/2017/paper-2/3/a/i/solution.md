<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $\kappa=|k|$. The differential operator in the [modified Helmholtz equation](../../../../../../modified-helmholtz-equation.md) depends only on $k^2=\kappa^2$. Let $G$ be its decaying [Green function](../../../../../../green-s-function-split.md). Acting on the proposed integral with the operator, in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md), gives

$$
\begin{aligned}
(\nabla_{\mathbf r}^2-k^2)\phi(\mathbf r)
&=\int_{\mathbb R^3}(\nabla_{\mathbf r}^2-k^2)G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'\\
&=\int_{\mathbb R^3}\delta^{(3)}(\mathbf r-\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'\\
&=\rho(\mathbf r).
\end{aligned}
$$

The last step is the sifting property of the [Dirac delta](../../../../../../dirac-delta-function.md). Thus

$$
\boxed{\phi(\mathbf r)=\int_{\mathbb R^3}G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'.}
$$

For a regular rapidly decaying source, the $1/|\mathbf r-\mathbf r'|$ singularity of the kernel found in part (ii) is locally [integrable](../../../../../../integrability.md) in three dimensions, and its convolution with the source tends to zero at infinity. This verifies both the equation and the decay condition. The sign of the kernel below corresponds to $\nabla^2-k^2$; reversing the sign of the entire operator reverses the kernel.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
