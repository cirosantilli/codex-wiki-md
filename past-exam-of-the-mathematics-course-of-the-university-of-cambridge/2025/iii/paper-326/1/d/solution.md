<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $p\in\partial J(v)$, the [Bregman divergence](../../../../../../bregman-divergence.md) is

$$
D_J^p(u,v)=J(u)-J(v)-\langle p,u-v\rangle.
$$

Put $r=A\widehat u_{\alpha,\delta}-f^\delta$ and $e=f^\delta-f$, so $\|e\|_Y\leq\delta$. Comparison with $u^\dagger$ gives

$$
\|r\|_Y+\alpha J(\widehat u_{\alpha,\delta})
\leq\delta+\alpha J(u^\dagger).
$$

Using $p^\dagger=A^*w^\dagger$,

$$
\begin{aligned}
D_J^{p^\dagger}(\widehat u_{\alpha,\delta},u^\dagger)
&=J(\widehat u_{\alpha,\delta})-J(u^\dagger)
-\langle w^\dagger,r+e\rangle\\
&\leq
\left(\frac1\alpha+\|w^\dagger\|_{Y^*}\right)\delta
+\left(\|w^\dagger\|_{Y^*}-\frac1\alpha\right)\|r\|_Y.
\end{aligned}
$$

For $0<\alpha<\alpha_0$ the last coefficient is negative, so

$$
\boxed{
D_J^{p^\dagger}(\widehat u_{\alpha,\delta},u^\dagger)
\leq C_\alpha\delta,
\qquad
C_\alpha=\frac1\alpha+\|w^\dagger\|_{Y^*}}.
$$

The estimate holds for any fixed admissible $\alpha$; it does not require $\alpha\to0$ with the noise level.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
