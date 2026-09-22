<h1 id="1/1/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It is sufficient that

$$
\boxed{0<\tau<\frac{2}{\|A\|^2}},
$$

and that the stopping rule obey

$$
k(\delta)\longrightarrow\infty,
\qquad
\delta\sqrt{k(\delta)}\longrightarrow0.
$$

For example, $k(\delta)=\lfloor\delta^{-1}\rfloor$ works.

For exact data $f\in\mathcal D(A^\dagger)$, each factor $(1-\tau\sigma_i^2)^k$ tends to zero. The [Picard criterion](../../../../../../../../picard-criterion.md) makes $\langle f,y_i\rangle/\sigma_i$ square summable, while $|1-(1-\tau\sigma_i^2)^k|$ is uniformly bounded. The [dominated convergence theorem](../../../../../../../../dominated-convergence-theorem.md) on the resulting series yields $u_k(f)\to A^\dagger f$.

For noisy data with $\|f^\delta-f\|\leq\delta$, the filter representation gives

$$
\|u_k(f^\delta)-u_k(f)\|
\leq
\delta\sup_{0<\sigma\leq\|A\|}
\frac{|1-(1-\tau\sigma^2)^k|}{\sigma}
\leq C_\tau\delta\sqrt{k}.
$$

Indeed, when $\tau\sigma^2\leq1$, [Bernoulli's inequality](../../../../../../../../bernoulli-s-inequality.md) gives $1-(1-\tau\sigma^2)^k\leq\min(k\tau\sigma^2,1)$; when $\tau\sigma^2>1$, the quotient is uniformly bounded because $\tau\|A\|^2<2$. Hence the [triangle inequality](../../../../../../../../triangle-inequality.md) gives

$$
\|u_{k(\delta)}(f^\delta)-A^\dagger f\|
\leq C_\tau\delta\sqrt{k(\delta)}
+\|u_{k(\delta)}(f)-A^\dagger f\|
\longrightarrow0,
$$

which proves that early-stopped Landweber iteration is a [convergent regularization of an inverse problem](../../../../../../../../convergent-regularization-of-an-inverse-problem.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [1](../../../../1.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2021](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
