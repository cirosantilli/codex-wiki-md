<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The affine class $C_\psi=\psi+H_0^1(\Omega)$ is nonempty, and part (i) gives a finite comparison energy $\mathcal F(\psi)$. Since $F(p)\geq\alpha|p|^2$, its energy infimum $m$ satisfies $0\leq m\leq\mathcal F(\psi)$. Choose a [minimizing sequence](../../../../../../minimizing-sequence.md) $u_k\in C_\psi$ with $\mathcal F(u_k)\leq\mathcal F(\psi)+1$. Then

$$
\alpha\|Du_k\|_2^2\leq\mathcal F(u_k)\leq\mathcal F(\psi)+1.
$$

The [gradient](../../../../../../gradient.md) bounds also control the full [Sobolev norm](../../../../../../sobolev-norm.md). Indeed $w_k=u_k-\psi\in H_0^1$, so the [Poincaré inequality](../../../../../../poincare-inequality.md) gives

$$
\|u_k\|_2\leq\|\psi\|_2+\|w_k\|_2\leq\|\psi\|_2+C_\Omega\bigl(\|Du_k\|_2+\|D\psi\|_2\bigr).
$$

Thus $u_k$ is bounded in the [Hilbert space](../../../../../../hilbert-space-split.md) $H^1(\Omega)$. Its weak compactness yields a weakly convergent subsequence $u_k\rightharpoonup u$. The closed linear subspace $H_0^1$ is weakly closed, hence $u-\psi\in H_0^1$ and $u\in C_\psi$. By part (ii),

$$
m\leq\mathcal F(u)\leq\liminf_k\mathcal F(u_k)=m.
$$

The [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md) therefore proves

$$
\boxed{u\in C_\psi,\qquad\mathcal F(u)=\min_{v\in C_\psi}\mathcal F(v).}
$$

Neither a smooth boundary nor a classical trace theorem is needed: the boundary condition is encoded by the closed [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
