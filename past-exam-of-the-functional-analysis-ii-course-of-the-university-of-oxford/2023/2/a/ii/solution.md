<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Composition with $t\mapsto t^{1+\alpha_n}$ preserves continuity, so $A_n$ maps the [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md) $C([0,1])$ into itself and is linear. Since $t\mapsto t^{1+\alpha_n}$ maps $[0,1]$ onto itself,

$$
\|A_nx\|_\infty=\|x\|_\infty,\qquad\|A_n\|=1.
$$

For $0<t\leq1$, the [mean value theorem](../../../../../mean-value-theorem.md) applied to $r\mapsto t^{1+r}$ gives

$$
0\leq t-t^{1+\alpha_n}\leq\alpha_n\,t|\log t|\leq\frac{\alpha_n}{e}.
$$

The same bound holds at $t=0$. Each $x\in C([0,1])$ has [uniform continuity](../../../../../uniform-continuity.md) by the [Heine-Cantor theorem](../../../../../heine-cantor-theorem.md). With its [modulus of continuity](../../../../../modulus-of-continuity.md) $\omega_x(\delta)=\sup_{|s-t|\leq\delta}|x(s)-x(t)|$, we obtain

$$
\boxed{\|A_nx-x\|_\infty\leq\omega_x(\alpha_n/e)\longrightarrow0.}
$$

Alternatively, the bound proves convergence on every [polynomial](../../../../../polynomial-split.md); the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) makes these a [dense subset](../../../../../dense-set.md) of $C([0,1])$, and the [Banach-Steinhaus convergence theorem](../../../../../banach-steinhaus-convergence-theorem.md) with $\|A_n\|=1$ gives the same conclusion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
