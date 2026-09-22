<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\delta=\operatorname{dist}(\Omega',\partial\Omega)>0$. Choose a smooth cutoff $0\leq\eta\leq1$, equal to one on $\Omega'$, supported within its $\delta/2$ neighborhood, with $|D\eta|\leq C_n/\delta$. Such a cutoff is obtained by smoothing a distance cutoff; its support is [relatively compact](../../../../../../relatively-compact-subset.md) in $\Omega$. Let $0<|h|<\delta/8$, fix a coordinate $k$, and put $z=\Delta_k^h u$. It lies in $W^{1,2}$ on the cutoff neighborhood because both translated copies of $u$ do. Extend $\eta^2z$ by zero, and use the [test function](../../../../../../test-function.md)

$$
\phi=-\Delta_k^{-h}(\eta^2z)\in W_0^{1,2}(\Omega).
$$

The weak equation is $\int Du\cdot D\phi=-\int f\phi$. The discrete integration-by-parts identity $\int a\Delta_k^{-h}b=-\int(\Delta_k^h a)b$, valid by translation with these supports, turns it into

$$
\int Dz\cdot D(\eta^2z)=\int f\Delta_k^{-h}(\eta^2z).
$$

Write $X=\|\eta Dz\|_2$, $U=\|z\|_{L^2(\operatorname{supp}\eta)}$, $A=\|D\eta\|_\infty$ and $F=\|f\|_2$. Expanding the left side gives $X^2$ plus a cross term of absolute value at most $2AUX$. Applying part (a) on the whole space to the zero extension of $\eta^2z$ bounds the right side by

$$
F\|D_k(\eta^2z)\|_2\leq F(X+2AU).
$$

Consequently

$$
X^2\leq(2AU+F)X+2AUF\leq\tfrac12X^2+C(A^2U^2+F^2),
$$

where the last step is the elementary [Young inequality](../../../../../../young-s-inequality-for-products.md). Part (a), on a slightly larger cutoff neighborhood if needed, gives $U\leq\|D_k u\|_{L^2(\Omega)}$. We conclude that

$$
\|D\Delta_k^h u\|_{L^2(\Omega')}\leq C_n\left(\|f\|_{L^2(\Omega)}+\delta^{-1}\|Du\|_{L^2(\Omega)}\right)
$$

uniformly as $h\to0$.

To obtain actual second [weak derivatives](../../../../../../weak-derivative.md), choose $h_j\to0$. For each $i,k$, the bounded sequence $\Delta_k^{h_j}D_i u$ has a [weakly convergent](../../../../../../weak-convergence.md) subsequence in $L^2(\Omega')$, say to $g_{ik}$. For every smooth compactly supported $\psi$ in $\Omega'$,

$$
\int g_{ik}\psi=\lim_j\int(\Delta_k^{h_j}D_i u)\psi
=-\lim_j\int D_i u\,\Delta_k^{-h_j}\psi=-\int D_i uD_k\psi.
$$

Thus $g_{ik}=D_kD_i u$ is the second [weak derivative](../../../../../../weak-derivative.md). [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) gives the same uniform bound for these derivatives. Adding the already known zeroth and first derivative norms and summing over the finitely many coordinates proves

$$
\boxed{u\in W_{\mathrm{loc}}^{2,2}(\Omega),\qquad
\|u\|_{W^{2,2}(\Omega')}\leq C(n,\delta)\bigl(\|u\|_{W^{1,2}(\Omega)}+\|f\|_{L^2(\Omega)}\bigr).}
$$

All derivative existence and estimates have been established by the difference-quotient argument; no second derivatives were assumed in choosing the test. This proves the [Interior second-derivative estimate for the Poisson equation](../../../../../../interior-second-derivative-estimate-for-the-poisson-equation.md) in the stated setting.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
