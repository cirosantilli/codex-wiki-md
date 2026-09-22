<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the interior [ordered subsolution and supersolution](../../../../../../ordered-subsolution-and-supersolution.md) correction from part (a). Recursively solve the [Poisson equation](../../../../../../poisson-equation.md) $\Delta u_{k+1}=V(u_k)$ with boundary value $\psi$, starting from $u_0=\varphi^-$. Part (a) gives $u_0\leq u_1\leq\varphi^+$. If $u_{k-1}\leq u_k\leq\varphi^+$, then

$$
\Delta(u_{k+1}-u_k)=V(u_k)-V(u_{k-1})\leq0,\qquad
\Delta(\varphi^+-u_{k+1})\leq V(\varphi^+)-V(u_k)\leq0.
$$

The first difference has zero boundary values, the second nonnegative values. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) applied to their negatives gives $u_k\leq u_{k+1}\leq\varphi^+$. Induction proves the bounded [monotone sequence](../../../../../../monotone-sequence.md)

$$
\boxed{\varphi^-\leq u_1\leq u_2\leq\cdots\leq\varphi^+.}
$$

Without interior ordering, the counterexample in part (a) disproves the claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
