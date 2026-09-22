<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove [compactness of zero-boundary Poisson solutions](../../../../../../compactness-of-zero-boundary-poisson-solutions.md). Here the printed $\partial\Omega$ must mean $\partial B_1$; otherwise the boundary condition refers to an unspecified set. Use this intended boundary condition throughout. Let $f=\Delta u$. A maximum-principle barrier gives a uniform bound on $u$: with $\psi(x)=(1-|x|^2)/(2n)$, we have $\Delta\psi=-1$ and $\psi=0$ on $\partial B_1$. Since $|f|\leq1$,

$$
\Delta(u-\psi)=f+1\geq0,\qquad\Delta(-u-\psi)=-f+1\geq0.
$$

The [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md) gives $-\psi\leq u\leq\psi$, so $\|u\|_\infty\leq1/(2n)$.

Standard [elliptic regularity](../../../../../../elliptic-regularity.md) on the smooth ball first gives $u\in C^{2,\mu}(\overline{B_1})$. The [global Schauder estimate](../../../../../../global-schauder-estimate.md) then gives

$$
\|u\|_{C^{2,\mu}(\overline{B_1})}\leq C\left(\|u\|_{C^0(\overline{B_1})}+\|f\|_{C^{0,\mu}(\overline{B_1})}\right)\leq C\left(1+\frac1{2n}\right).
$$

Thus the functions and all their derivatives through order two are uniformly bounded and [equicontinuous](../../../../../../equicontinuity.md) on the closed ball. The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) gives a subsequence converging uniformly along with all these derivatives. Integration along line segments identifies the limiting derivatives, so the convergence is in $C^2(\overline{B_1})$.

It remains to keep the limit in the set, rather than merely proving [relative compactness](../../../../../../relatively-compact-subset.md). If $u_j\to u$ in $C^2$, then the zero boundary values pass to the limit and $f_j=\Delta u_j\to f=\Delta u$ uniformly. For each pair of distinct points,

$$
\frac{|f(x)-f(y)|}{|x-y|^\mu}=\lim_j\frac{|f_j(x)-f_j(y)|}{|x-y|^\mu}.
$$

Taking suprema gives $[f]_\mu\leq\liminf_j[f_j]_\mu$, while $\|f_j\|_\infty\to\|f\|_\infty$. Hence $\|f\|_{C^{0,\mu}}\leq1$. The limit belongs to the set, proving **[sequential compactness](../../../../../../sequentially-compact-space.md) in $C^2(\overline{B_1})$**. The fixed positive Hölder exponent supplies the compactness; a bound on the [supremum norm](../../../../../../supremum-norm.md) of $\Delta u$ alone would not supply this argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
