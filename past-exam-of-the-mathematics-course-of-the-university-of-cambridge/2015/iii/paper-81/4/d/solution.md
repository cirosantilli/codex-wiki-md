<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $K=H-\mu N$, take $M$ slices of width $\epsilon=\beta/M$, and insert the [coherent-state resolution of identity](../../../../../../coherent-state-resolution-of-identity.md) between factors of $e^{-\epsilon K}$. If $H$ is in [normal ordering](../../../../../../normal-ordering.md), each short-time matrix element is

$$
\langle\psi_{j+1}|e^{-\epsilon K}|\psi_j\rangle=\exp\left[\sum_n\bar\psi_{n,j+1}\psi_{n,j}-\epsilon K(\bar\psi_{j+1},\psi_j)+O(\epsilon^2)\right].
$$

Combining the overlap with the Gaussian weight leaves $\sum_{j,n}\bar\psi_{n,j}(\psi_{n,j}-\psi_{n,j-1})$ in the action. The [coherent-state time slicing](../../../../../../coherent-state-time-slicing.md) prescription fixes which adjacent labels appear in $H$, rather than allowing an arbitrary ordering change after taking the continuum limit.

The twist $\zeta$ in the thermal trace closes the path with the [coherent-state thermal boundary conditions](../../../../../../coherent-state-thermal-boundary-conditions.md): periodic for bosons, antiperiodic for fermions. Taking the regulated continuum limit gives

$$
\boxed{Z=\int_{\psi(\beta)=\zeta\psi(0),\ \bar\psi(\beta)=\zeta\bar\psi(0)}\mathcal D(\bar\psi,\psi)\,e^{-\mathcal S},\qquad \mathcal S=\int_0^\beta d\tau\left[\sum_n\bar\psi_n(\partial_\tau-\mu)\psi_n+H(\bar\psi,\psi)\right]}.
$$

The action is dimensionless because $\tau$ has inverse-energy units. For fermions, $\bar\psi$ and $\psi$ remain independent [Grassmann fields](../../../../../../grassmann-field.md). If the original [Hamiltonian](../../../../../../hamiltonian.md) is not normally ordered, first express it in normal order, retaining all constants.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
