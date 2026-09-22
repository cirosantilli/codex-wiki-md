<h1 id="32c/solution">Solution</h1>

↑ **Parent:** [32C](../32c.md)

Define the [interaction picture](../../../../../interaction-picture.md) by $|\psi_I(t)\rangle=e^{iH_0t/\hbar}|\psi_S(t)\rangle$. Differentiating and using the [Schrödinger equation](../../../../../schrodinger-equation.md) cancels the free Hamiltonian:

$$
i\hbar\frac d{dt}|\psi_I(t)\rangle
=V_I(t)|\psi_I(t)\rangle,\qquad
V_I(t)=e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}.
$$

Integrating once and replacing the state in the integral by its initial value gives

$$
|\psi_I(t)\rangle=|a\rangle-\frac i\hbar\int_0^tV_I(t')|a\rangle\,dt'
+O(V^2).
$$

Since $\langle b|a\rangle=0$, the first-order transition amplitude is $-i/\hbar$ times the integral of $\langle b|V(t')|a\rangle e^{i(E_b-E_a)t'/\hbar}$. Its modulus squared gives

$$
\boxed{P_{a\to b}(t)=\frac1{\hbar^2}
\left|\int_0^t\langle b|V(t')|a\rangle
e^{i(E_b-E_a)t'/\hbar}\,dt'\right|^2}
$$

to second order in the perturbation.

For the two-state example, the matrix element is $vt'$ and the free energies coincide. Thus $P_{1\to2}=v^2t^4/(4\hbar^2)$ to order $v^2$. All Hamiltonians commute at different times because they are combinations of $I$ and the same [Pauli matrix](../../../../../pauli-matrices.md) $\sigma_1$. Therefore the ordinary exponential of their time integral solves the equation: differentiating it gives $-(i/\hbar)(EI+vt\sigma_1)$ times itself, and its value at zero is $I$. Since $\sigma_1^2=I$, it is

$$
e^{-iEt/\hbar}\left[\cos\left(\frac{vt^2}{2\hbar}\right)I
-i\sin\left(\frac{vt^2}{2\hbar}\right)\sigma_1\right].
$$

Starting from state 1, the exact result and the approximation condition are

$$
\boxed{P_{1\to2}(t)=\sin^2\left(\frac{vt^2}{2\hbar}\right),\qquad
\left|\frac{vt^2}{2\hbar}\right|\ll1.}
$$

## ↑ Ancestors (10)

1. [32C](../32c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
