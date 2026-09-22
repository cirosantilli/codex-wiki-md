<h1 id="3/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the complete-data model as $p_\theta(y\mid a)$ and the missingness model as $q_\psi(r\mid y,a)$. Under MAR,

$$
q_\psi(r\mid y,a)=q_\psi(r\mid y_{\mathrm{obs}},a).
$$

Therefore the observed-data likelihood factorizes as

$$
\begin{aligned}
L(\theta,\psi)
&=\int p_\theta(y_{\mathrm{obs}},y_{\mathrm{mis}}\mid a)
q_\psi(r\mid y_{\mathrm{obs}},a)\,dy_{\mathrm{mis}}\\
&=q_\psi(r\mid y_{\mathrm{obs}},a)
\int p_\theta(y_{\mathrm{obs}},y_{\mathrm{mis}}\mid a)
\,dy_{\mathrm{mis}}.
\end{aligned}
$$

With distinct parameters, the first factor does not involve $\theta$. Maximizing or integrating the second factor therefore gives the same likelihood inference for $\theta$ as modeling the missingness process explicitly. Hence **MAR plus distinctness makes missingness ignorable**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
