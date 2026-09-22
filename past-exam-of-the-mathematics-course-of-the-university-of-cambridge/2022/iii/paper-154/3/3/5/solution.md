<h1 id="3/3/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Part 3 and [Mass conservation for the nonlinear Schrödinger equation](../../../../../../../mass-conservation-for-the-nonlinear-schrodinger-equation.md) give

$$
\|v_n\|_2=\|Q\|_2,\qquad
\|\nabla v_n\|_2=\|\nabla Q\|_2,\qquad
E(v_n)\to0.
$$

The last relation and the energy formula imply

$$
\|v_n\|_{2+4/d}^{2+4/d}
\longrightarrow\frac{2+4/d}{2}\|\nabla Q\|_2^2
=\|Q\|_{2+4/d}^{2+4/d},
$$

where the final equality follows from the [Pohozaev identity for the mass-critical NLS ground state](../../../../../../../pohozaev-identity-for-the-mass-critical-nls-ground-state.md). Thus $(v_n)$ is a minimizing sequence for the [Weinstein functional](../../../../../../../weinstein-functional.md) with the same normalization as $Q$.

Apply the profile decomposition from part 4. The [Sharp Gagliardo-Nirenberg inequality](../../../../../../../sharp-gagliardo-nirenberg-inequality.md) bounds each profile by the product of its gradient energy and its mass to the power $2/d$. Since the total mass is exactly $\|Q\|_2^2$, any split into two nonzero profiles would make the limiting inequality strict. Hence precisely one profile carries all the mass and gradient energy. The norm decouplings then make the remainder converge strongly to zero in $H^1$. For suitable translations $x_n$,

$$
v_n(\,\cdot+x_n)\longrightarrow\phi
\quad\text{strongly in }H^1(\mathbb R^d),
$$

and the [Sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md) gives the required strong convergence in $L^{2+4/d}$. This is the [compactness of a mass-critical minimizing sequence](../../../../../../../compactness-of-a-mass-critical-minimizing-sequence.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
