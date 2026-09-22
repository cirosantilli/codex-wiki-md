<h1 id="23f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Subtracting the global weighted mean from $h$ leaves its derivative unchanged, so it suffices to assume

$$
\int_{\mathbb R}he^{-\Phi}=0.
$$

Write $w=e^{-\Phi}$, choose $R\geq R_0$, and put

$$
I=\int_{|x|\leq R}|h|^2w,
\qquad
O=\int_{|x|>R}|h|^2w,
\qquad
Z=\int_{|x|\leq R}w,
\qquad
q=1-Z.
$$

The weighted mean of $h$ on $[-R,R]$ is

$$
a=\frac1Z\int_{|x|\leq R}hw=-\frac1Z\int_{|x|>R}hw.
$$

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
Z|a|^2\leq\frac qZ O.
$$

Part (c), applied on $[-R,R]$, therefore gives for $E=\int_{\mathbb R}|h'|^2w$

$$
E\geq\lambda_R\int_{|x|\leq R}|h-a|^2w
=\lambda_R(I-Z|a|^2)
\geq\lambda_R I-\lambda_R\frac qZ O.
$$

Part (a) gives independently

$$
E\geq\lambda_1O-K_1I.
$$

Choose $\epsilon_0>0$ so small that $\epsilon_0K_1\leq1/2$, and then choose $R$ large enough that $q/Z\leq\epsilon_0\lambda_1/2$. Multiply the last inequality by $\epsilon=\epsilon_0\lambda_R$ and add it to the local inequality. This yields

$$
(1+\epsilon)E
\geq\frac{\lambda_R}{2}I
+\frac{\epsilon_0\lambda_R\lambda_1}{2}O
\geq c_R(I+O),
$$

where $c_R=\frac{\lambda_R}{2}\min\{1,\epsilon_0\lambda_1\}>0$. Hence, with $\lambda_0=c_R/(1+\epsilon)$,

$$
\boxed{
\int_{\mathbb R}|h'|^2e^{-\Phi}
\geq\lambda_0\int_{\mathbb R}\left|h-\int_{\mathbb R}he^{-\Phi}\right|^2e^{-\Phi}
}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
