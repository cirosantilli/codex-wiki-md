<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N=|V_n|$. Since the degrees lie between $1$ and $\Delta$,

$$
\pi_{\min}\geq\frac1{\Delta N}.
$$

The [Generalized Cheeger inequality](../../../../../../generalized-cheeger-inequality.md) and $\Phi_*(u)\geq\Phi_*(c)\geq\alpha$ for $u\leq c$ give

$$
\Lambda(u)\geq\frac{\alpha^2}{2}
\qquad(\pi_{\min}\leq u\leq c).
$$

For all larger $u$, part (a) gives $\Lambda(u)\geq1/t_{\mathrm{rel}}$. Split the supplied spectral-profile integral at $c$ to obtain

$$
\begin{aligned}
t_{\mathrm{mix}}(\varepsilon)
&\leq2\int_{4\pi_{\min}}^{4/\varepsilon}\frac{du}{u\Lambda(u)}\\
&\lesssim_{\alpha,c,\Delta}
\log\frac1{\pi_{\min}}+t_{\mathrm{rel}}\log\frac1\varepsilon\\
&\lesssim\log N+t_{\mathrm{rel}}\log(1/\varepsilon).
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
