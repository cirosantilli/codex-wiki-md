<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiply $\Delta u+qu\leq0$ by $\zeta^2/u_\varepsilon$ and integrate. Since $\zeta$ is compactly supported, [integration by parts](../../../../../../../integration-by-parts.md) and Young's inequality give

$$
\begin{aligned}
\int q\frac{u}{u_\varepsilon}\zeta^2
&\leq-\int\frac{\Delta u}{u_\varepsilon}\zeta^2\\
&=2\int\frac{\zeta Du\cdot D\zeta}{u_\varepsilon}
-\int\frac{\zeta^2|Du|^2}{u_\varepsilon^2}\\
&\leq\int|D\zeta|^2.
\end{aligned}
$$

As $\varepsilon\downarrow0$, $u/u_\varepsilon$ converges to the indicator of $\{u>0\}$. The [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) therefore gives

$$
\boxed{\int_{\{u>0\}}q\zeta^2\leq\int|D\zeta|^2.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
