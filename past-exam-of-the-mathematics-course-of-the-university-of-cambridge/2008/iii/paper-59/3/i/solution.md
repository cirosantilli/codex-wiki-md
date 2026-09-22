<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [Lagrangian mechanics](../../../../../../lagrangian-mechanics.md), let a one-parameter group on $Q$ have generator $\xi_Q=\xi^i(q)\partial_{q^i}$. Its tangent lift acts on $TQ$ as

$$
\xi_{TQ}=\xi^i\partial_{q^i}+v^j\partial_j\xi^i\partial_{v^i}.
$$

If $L$ is invariant, $\xi_{TQ}L=0$. Along an Euler–Lagrange trajectory, the [Noether conserved quantity for a mechanical point symmetry](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) is

$$
J^L_\xi=\theta_L(\xi_{TQ})=\frac{\partial L}{\partial v^i}\xi^i,
$$

because

$$
\frac{dJ^L_\xi}{dt}=\dot p_i\xi^i+p_i\partial_j\xi^i v^j=L_{q^i}\xi^i+L_{v^i}\partial_j\xi^iv^j=\xi_{TQ}L=0.
$$

Thus the [conserved quantity](../../../../../../conserved-quantity.md) is explicitly derived, not merely attached to the name of a [symmetry](../../../../../../symmetry-physics.md). If the change of $L$ is the total derivative $dB/dt$, then $p_i\xi^i-B$ is conserved. For a general point transformation with time component $\tau$, the conserved expression is $p_i\xi^i-E_L\tau-B$, provided the variation of $L\,dt$ is $dB$. Time-translation invariance of an autonomous Lagrangian therefore yields conservation of energy.

In [Hamiltonian mechanics](../../../../../../hamiltonian-mechanics.md), a cotangent-lifted action preserves $\theta$ and hence $\omega$. For its infinitesimal generator $\xi_{T^*Q}$, [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) gives

$$
0=\mathcal L_{\xi_{T^*Q}}\theta=\iota_{\xi_{T^*Q}}d\theta+d(\theta(\xi_{T^*Q})),\qquad\iota_{\xi_{T^*Q}}\omega=dJ_\xi,
$$

where $J_\xi=p_i\xi^i$. These components define the canonical [moment map](../../../../../../moment-map.md) $J:T^*Q\to\mathfrak g^*$, with $\langle J,\xi\rangle=J_\xi$. If $H$ is invariant, $\{H,J_\xi\}=0$, so $\dot J_\xi=\{J_\xi,H\}=0$. This is the Hamiltonian form of [Noether's theorem](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md), and the [Legendre transform in mechanics](../../../../../../legendre-transform-in-mechanics.md) identifies its charges with the Lagrangian ones.

More generally, a [Hamiltonian group action](../../../../../../hamiltonian-group-action.md) is an action whose infinitesimal symplectic generators have globally defined Hamiltonian functions. The existence of those functions is an assumption, not a consequence of every symplectic action. For example, translation on a symplectic two-torus preserves $dq\wedge dp$ but contraction with $\partial_q$ gives $dp$, which is closed and not globally exact. Such a [symmetry](../../../../../../symmetry-physics.md) need not have a globally single-valued moment-map component. On $T^*Q$, the cotangent lift does have the canonical components just derived. **A Hamiltonian [symmetry](../../../../../../symmetry-physics.md) preserving $H$ gives a conserved generator; the global momentum-map hypotheses must be stated.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
