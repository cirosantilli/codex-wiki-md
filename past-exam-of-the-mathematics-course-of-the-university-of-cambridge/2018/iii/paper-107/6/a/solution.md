<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**As printed, the hypotheses are insufficient.** They order the barriers only on the boundary; the intended [monotone iteration for a semilinear elliptic equation](../../../../../../monotone-iteration-for-a-semilinear-elliptic-equation.md) needs an [ordered subsolution and supersolution](../../../../../../ordered-subsolution-and-supersolution.md) throughout the domain. On $B_1$, take a positive first [Dirichlet Laplacian eigenfunction](../../../../../../dirichlet-laplacian-eigenfunction.md) $e_1$ with $-\Delta e_1=\lambda_1e_1$, and set

$$
V(s)=-\lambda_1s,\qquad \psi=0,\qquad \varphi^-=e_1,\qquad \varphi^+=-e_1.
$$

Both barriers satisfy $Q\varphi^\pm=0$ and vanish on the boundary, but $\varphi^->\varphi^+$ inside. No function lies between them. This also disproves the unconditional conclusions in (b) and (d).

With the intended extra hypothesis $\varphi^-\leq\varphi^+$ on $\overline\Omega$, solvability of the [Poisson equation](../../../../../../poisson-equation.md) and the [Schauder estimate](../../../../../../schauder-estimates.md) give a unique $u_1\in C^{2,\alpha}$ with forcing $V(\varphi^-)$ and boundary data $\psi$. Smooth $V$ composed with the $C^{0,\alpha}$ barrier has the required forcing regularity. The barrier inequalities give

$$
\Delta(u_1-\varphi^-)=V(\varphi^-)-\Delta\varphi^-\leq0,
\qquad
\Delta(\varphi^+-u_1)\leq V(\varphi^+)-V(\varphi^-)\leq0.
$$

Both differences have nonnegative boundary values. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) applied to their negatives gives $\boxed{\varphi^-\leq u_1\leq\varphi^+}$ under the corrected hypothesis.

## ↑ Ancestors (11)

1. [A](../a.md)
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
