<h1 id="32b/solution">Solution</h1>

↑ **Parent:** [32B](../32b.md)

[Hamilton's equations](../../../../../hamilton-s-equations.md) are $\dot q_j=\partial H/\partial p_j$ and $\dot p_j=-\partial H/\partial q_j$. The [Arnold-Liouville theorem](../../../../../liouville-arnold-theorem.md) states that $n$ functionally independent first integrals in involution on a $2n$-dimensional [symplectic manifold](../../../../../symplectic-manifold.md) give local integrability; a compact connected regular common level is an $n$-torus. Near such a torus there are [action-angle variables](../../../../../action-angle-variables.md) $(I,\vartheta)$ with $H=H(I)$, $\dot I=0$ and $\dot\vartheta=\partial H/\partial I$.

For the displayed diagonal oscillator [Hamiltonian](../../../../../hamiltonian.md) set $E_k=(p_k^2+\omega_k^2q_k^2)/2$. Each is constant, since $\dot q_k=p_k$ and $\dot p_k=-\omega_k^2q_k$. Different $E_k$ depend on disjoint canonical pairs, so their [Poisson brackets](../../../../../poisson-bracket.md) vanish. Their differentials are independent wherever every $dE_k$ is nonzero, an open dense set; this proves complete integrability. For nonzero frequencies put $\Omega_k=|\omega_k|$. A positive-energy level in each pair is an ellipse with semiaxes $\sqrt{2E_k}$ and $\sqrt{2E_k}/\Omega_k$. Its enclosed area is $2\pi E_k/\Omega_k$, so the [action variables](../../../../../action-variable.md) are

$$
\boxed{I_k=\frac1{2\pi}\oint p_k\,dq_k=\frac{E_k}{|\omega_k|},\qquad H=\sum_k|\omega_k|I_k.}
$$

For the usual positive oscillator frequencies this is $I_k=E_k/\omega_k$. If a printed “constant” frequency is allowed to be zero, that pair is a free particle: $p_k$ is a commuting integral, but its generic level is noncompact and has no closed-cycle oscillator action. Complete integrability persists, while the torus/action formula requires nonzero frequencies.

## ↑ Ancestors (10)

1. [32B](../32b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
