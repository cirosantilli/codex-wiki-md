<h1 id="31c/solution">Solution</h1>

↑ **Parent:** [31C](../31c.md)

A [Hamiltonian system](../../../../../hamiltonian-system.md) with $n$ [degrees of freedom](../../../../../degree-of-freedom.md) is [Liouville integrable](../../../../../integrable-hamiltonian-system.md) if it has $n$ functionally independent [first integrals](../../../../../first-integral.md), including the [Hamiltonian](../../../../../hamiltonian.md), whose pairwise [Poisson brackets](../../../../../poisson-bracket.md) vanish. [Functional independence](../../../../../functionally-independent-functions.md) is required on a regular open set. The [Arnold-Liouville theorem](../../../../../liouville-arnold-theorem.md) says that a connected compact regular common level of these integrals is an $n$-torus, with a neighborhood admitting [action-angle coordinates](../../../../../action-angle-variables.md); the [Hamiltonian](../../../../../hamiltonian.md) flow there has constant angular velocities and fixed actions. Compactness is essential to the torus conclusion.

Use $\{f,g\}=\sum_j(f_{q_j}g_{p_j}-f_{p_j}g_{q_j})$. On $r>0$, for differentiable $F$, [Hamilton's equations](../../../../../hamilton-s-equations.md) give $\dot q=p$, $\dot p=-F'(r)q/r$. Hence the [angular momentum](../../../../../angular-momentum.md) $M=q\times p$ obeys

$$
\dot M=\dot q\times p+q\times\dot p=p\times p-\frac{F'(r)}r q\times q=0.
$$

In particular $M_1$ and $M_2$ are [first integrals](../../../../../first-integral.md). The [Jacobi identity for the Poisson bracket](../../../../../jacobi-identity-for-the-poisson-bracket.md) is

$$
\{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0.
$$

Taking $f=H,g=M_1,h=M_2$ shows $\{H,\{M_1,M_2\}\}=0$. Direct differentiation gives $M_3=\{M_1,M_2\}=q_1p_2-q_2p_1$ and, cyclically, $\{M_i,M_j\}=\epsilon_{ijk}M_k$.

Set $L^2=M_1^2+M_2^2+M_3^2$. Then $\{L^2,M_3\}=2M_1(-M_2)+2M_2M_1=0$, and the brackets of $H$ with both expressions vanish. Thus

$$
\boxed{H,\ L^2,\ M_3\text{ are three commuting first integrals}.}
$$

For [functional independence](../../../../../functionally-independent-functions.md), at $q=(r,0,0)$ with $r>0$ the [Jacobian matrix](../../../../../jacobian-matrix.md) of $(H,L^2,M_3)$ with respect to $(p_1,p_2,p_3)$ is

$$
\begin{pmatrix}p_1&p_2&p_3\\0&2r^2p_2&2r^2p_3\\0&r&0\end{pmatrix},
$$

whose [determinant](../../../../../determinant.md) is $-2r^3p_1p_3$. It is nonzero when $p_1p_3\ne0$. More generally this minor is a nonzero polynomial in $q,p$, independent of $F$, so its zero set has empty interior and the integrals are independent on a dense open regular set. This proves [Liouville integrability](../../../../../integrable-hamiltonian-system.md) on the regular set. The arbitrary potential in the question does not ensure compact common levels: $F=0$ has unbounded free trajectories. The full torus conclusion applies to those regular connected common levels which are compact, rather than to every choice of $F$ and every level.

## ↑ Ancestors (10)

1. [31C](../31c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
