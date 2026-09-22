<h1 id="2/2/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $\psi_R(x)=R^2\psi(x/R)$, the assumptions imply $\operatorname{Hess}\psi_R\leq I$, while on $|x|\leq2R$ one has

$$
\operatorname{Hess}\psi_R=I,
\qquad \Delta\psi_R=d,
\qquad \Delta^2\psi_R=0.
$$

Apply the [localized virial identity](../../../../../../../localized-virial-identity.md) and compare its interior terms with

$$
E(u)=\frac12\|\nabla u\|_2^2-
\frac1{p+1}\|u\|_{p+1}^{p+1}\leq0.
$$

The coefficient $d(p-1)/4$ is strictly greater than one because $s_c>0$. The resulting negative multiple of $\|\nabla u\|_2^2$ can be moved to the left. All errors in the nonlinear term are supported on $|x|\geq2R$, and $\Delta^2\psi_R=O(R^{-2})$ is supported on $2R\leq|x|\leq10R$. Thus

$$
\boxed{c(d,p)\int|\nabla u|^2
+\frac12\frac d{dt}V_{\psi_R}(t)
\leq C(d,p)\left[
\int_{|x|\geq2R}|u|^{p+1}
+\frac1{R^2}\int_{2R\leq|x|\leq10R}|u|^2
\right].}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
