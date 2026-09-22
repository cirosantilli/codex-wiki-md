<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The normalized [Hartree product state](../../../../hartree-product-state.md) and its equivalent [second quantization](../../../../second-quantization.md) form are

$$
\boxed{\Psi_{\theta,\chi}(\mathbf r_1,\ldots,\mathbf r_N)
=\prod_{j=1}^N\varphi_{(\theta,\chi)}(\mathbf r_j),\qquad
|\theta,\chi;N\rangle=\frac{(\cos\theta\,\hat a_L^\dagger+e^{i\chi}\sin\theta\,\hat a_R^\dagger)^N}{\sqrt{N!}}|0\rangle.}
$$

The product is already symmetric under exchanging [bosons](../../../../boson.md); no additional $1/\sqrt{N!}$ belongs in the coordinate [wavefunction](../../../../wave-function-split.md). The factor in the [second quantization](../../../../second-quantization.md) expression instead normalizes repeated [creation operators](../../../../creation-operator.md) acting on the [vacuum state](../../../../vacuum-state.md). This is a [fixed-number two-mode condensate](../../../../fixed-number-two-mode-condensate.md), with every [boson](../../../../boson.md) in the same normalized [orbital](../../../../single-particle-orbital.md).

Set $c=\cos\theta$ and $s=\sin\theta$. Its [binomial distribution](../../../../binomial-distribution.md) of occupations gives

$$
\langle\hat n_L\rangle=Nc^2,\quad\langle\hat n_R\rangle=Ns^2,\quad
\langle\hat a_L^\dagger\hat a_R\rangle=Ncs\,e^{i\chi},\qquad
\langle\hat n_L^2+\hat n_R^2\rangle=N+N(N-1)(c^4+s^4).
$$

The [expectation value](../../../../expectation-value.md) of the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is therefore

$$
\boxed{E(\theta,\chi)=-tN\sin(2\theta)\cos\chi
+w\left[N+N(N-1)\left(1-\frac12\sin^2(2\theta)\right)\right]-\mu N.}
$$

Keeping $N(N-1)$ rather than replacing it by $N^2$ retains the exact pair count of the trial [quantum state](../../../../quantum-state.md). Equivalently, with $\epsilon=w-\mu$, its interaction contribution is $wN(N-1)(c^4+s^4)$ and its one-particle contribution is $\epsilon N-tN\sin(2\theta)\cos\chi$.

Choose the nonredundant parameter range $0\leq\theta\leq\pi/2$, with $\chi$ modulo $2\pi$. For $t>0$, minimizing over the relative [phase](../../../../phase-waves.md) gives $\chi=0$. Putting $x=\sin(2\theta)\in[0,1]$, the remaining nonconstant [energy](../../../../energy-split.md) is $-tNx-\tfrac12wN(N-1)x^2$, which decreases with $x$ for the repulsive coupling $w>0$. Hence

$$
\boxed{\theta=\frac\pi4,\qquad\chi=0\pmod{2\pi},\qquad
E_{\min}=-tN+\frac w2N(N+1)-\mu N.}
$$

The optimal [orbital](../../../../single-particle-orbital.md) is the symmetric $\phi_0=(\varphi_L+\varphi_R)/\sqrt2$. Both the [quantum tunnelling](../../../../quantum-tunnelling.md) term and the repulsive interaction favor this balanced occupation within the [Hartree product state](../../../../hartree-product-state.md) family. This result uses a [variational method](../../../../variational-method.md): for strong repulsion relative to [quantum tunnelling](../../../../quantum-tunnelling.md), the true many-body [ground state](../../../../ground-state.md) can have smaller occupation fluctuations than this [fixed-number two-mode condensate](../../../../fixed-number-two-mode-condensate.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
