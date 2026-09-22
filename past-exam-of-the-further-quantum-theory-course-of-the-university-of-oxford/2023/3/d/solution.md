<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $V(-x)=V(x)$, the [parity operator](../../../../parity-operator.md) $P\psi(x)=\psi(-x)$ commutes with the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). Also $P^2=I$, so its [eigenvalues](../../../../eigenvalue.md) are $\pm1$ and the [energy eigenspaces](../../../../energy-eigenspace.md) admit a [basis](../../../../basis.md) of definite [parity](../../../../parity.md). More strongly, [nondegeneracy of one-dimensional bound states](../../../../nondegeneracy-of-one-dimensional-bound-states.md) says that each [bound state](../../../../bound-state.md) [energy](../../../../energy-split.md) here is nondegenerate: the [Wronskian](../../../../wronskian.md) of two solutions at the same [energy](../../../../energy-split.md) is constant by the [Schrödinger equation](../../../../schrodinger-equation.md), and decay at infinity makes it zero, forcing linear dependence. Thus each [bound state](../../../../bound-state.md) itself is even or odd.

An [even function](../../../../even-function.md) obeys the [Neumann boundary condition](../../../../neumann-boundary-condition.md) $\psi'(0)=0$; an [odd function](../../../../odd-function.md) obeys the [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) $\psi(0)=0$. Write

$$
K_0=\frac1\hbar\int_0^{x_1}\chi(x)\,dx,\qquad \phi(E)=2K_0=\frac1\hbar\int_{-x_1(E)}^{x_1(E)}\sqrt{2m[V(x)-E]}\,dx.
$$

Smooth reflection symmetry gives $\chi'(0)=0$, while $K'(0)=-\chi(0)/\hbar$. Hence, for the central [WKB approximation](../../../../wkb-approximation.md) from part (c),

$$
\psi_R(0)\simeq\frac{F}{\sqrt{\chi(0)}}\bigl[2\cos\theta\,e^{K_0}+\sin\theta\,e^{-K_0}\bigr],
$$



$$
\psi_R'(0)\simeq\frac{F\sqrt{\chi(0)}}\hbar\bigl[-2\cos\theta\,e^{K_0}+\sin\theta\,e^{-K_0}\bigr].
$$

The two [boundary conditions](../../../../boundary-condition.md) consequently give the [WKB quantization condition for a symmetric double well](../../../../wkb-quantization-condition-for-a-symmetric-double-well.md):

$$
\boxed{\tan\theta(E)=C_\pm e^{\phi(E)},\qquad C_+=2\ \text{for even parity},\qquad C_-=-2\ \text{for odd parity}.}
$$

The full [wavefunction](../../../../wave-function-split.md) is $\psi_+(x)=\psi_R(|x|)$ in the even case and $\psi_-(x)=\operatorname{sgn}(x)\psi_R(|x|)$ in the odd case, with the value at zero fixed continuously. The relevant [boundary condition](../../../../boundary-condition.md) makes these extensions differentiable at zero. Both [action integrals](../../../../action-integral.md) $\theta,\phi$ depend on $E$ through the integrands and the [classical turning points](../../../../classical-turning-point.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
