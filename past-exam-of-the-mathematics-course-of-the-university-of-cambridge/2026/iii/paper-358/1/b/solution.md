<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $f\in C_c^\infty(\mathbb R)$, integration by parts gives

$$
\|Tf\|^2=\|f''\|^2+\|xf\|^2
+2\operatorname{Re}\langle-f'',ixf\rangle.
$$

Another integration by parts removes the factor $x$ from the real cross term and yields the bound

$$
|2\operatorname{Re}\langle-f'',ixf\rangle|
\leq2\|f'\|\|f\|.
$$

The Sobolev interpolation estimate $\|f'\|^2\leq\varepsilon\|f''\|^2+C_\varepsilon\|f\|^2$ therefore implies

$$
\boxed{\|f''\|^2+\|xf\|^2
\leq C(\|Tf\|^2+\|f\|^2)}.
$$

Thus convergence in the graph norm of the closure forces convergence in $H^2$ and of $xf$ in $L^2$. Conversely, $f\in H^2$ and $xf\in L^2$ clearly makes $-f''+ixf\in L^2$, and cutoff followed by mollification approximates it in this graph norm. Hence

$$
\boxed{D(T)=\{f\in H^2(\mathbb R):xf\in L^2(\mathbb R)\}}.
$$

The operator is accretive because

$$
\operatorname{Re}\langle Tf,f\rangle=\|f'\|^2.
$$

Consequently $T+I$ and its adjoint $T^*+I=-d^2/dx^2-ix+I$ are bounded below by one. The range of $T+I$ is both closed and dense, hence all of $L^2$, so $-1$ is a resolvent point. If $f=(T+I)^{-1}g$ with $\|g\|\leq1$, then $\|f\|\leq1$, and the graph estimate bounds $\|f''\|$ and $\|xf\|$. The compactness criterion in the question shows that $(T+I)^{-1}$ is compact. Thus the [Imaginary Airy operator](../../../../../../imaginary-airy-operator.md) has compact resolvent.

For the unitary translation $(U_af)(x)=f(x-a)$,

$$
U_a^{-1}TU_a=T+iaI.
$$

Therefore

$$
\boxed{\|(T-(z+ia)I)^{-1}\|
=\|(T-zI)^{-1}\|},
$$

so the inverse resolvent norm is constant on every vertical line. The same unitary equivalence gives $\sigma(T)=\sigma(T)+ia$ for every real $a$. If the spectrum contained one point, it would contain its entire vertical line, contradicting the isolated-point spectrum forced by compact resolvent. Hence

$$
\boxed{\sigma(T)=\varnothing}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
