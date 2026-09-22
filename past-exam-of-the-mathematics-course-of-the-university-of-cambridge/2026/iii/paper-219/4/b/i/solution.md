<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For any approximating density $q_\phi$,

$$
\begin{aligned}
\log Z
&=\mathbb E_{q_\phi}
\log\frac{L(\theta)\pi(\theta)}{q_\phi(\theta)}
+D_{\mathrm{KL}}(q_\phi\Vert p(\theta\mid y))\\
&=\operatorname{ELBO}(\phi)
+D_{\mathrm{KL}}(q_\phi\Vert p(\theta\mid y)).
\end{aligned}
$$

The [evidence lower bound](../../../../../../../evidence-lower-bound.md) is therefore

$$
\operatorname{ELBO}(\phi)
=\mathbb E_{q_\phi}\log L(\theta)
-D_{\mathrm{KL}}(q_\phi\Vert\pi).
$$

Since $\log Z$ does not depend on $\phi$, maximizing the ELBO is equivalent to minimizing the divergence from $q_\phi$ to the posterior.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
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
