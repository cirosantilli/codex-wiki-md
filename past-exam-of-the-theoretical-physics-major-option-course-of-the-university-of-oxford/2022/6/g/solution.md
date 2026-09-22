<h1 id="6/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For a free real [scalar field](../../../../scalar-field.md) in four spacetime dimensions, $\mathcal L=(\partial\phi)^2/2-m^2\phi^2/2$ and $\pi=\dot\phi$. Canonical quantization promotes these canonical fields to Hermitian operator-valued distributions with equal-time [canonical commutation relations](../../../../canonical-commutation-relation.md)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y),\qquad[\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

Expand the solution of the [Klein-Gordon equation](../../../../klein-gordon-equation.md) into positive- and negative-frequency modes:

$$
\phi(x)=\int d\Pi_k\,[a(\mathbf k)e^{-ikx}+a^\dagger(\mathbf k)e^{ikx}],\quad d\Pi_k=\frac{d^3k}{(2\pi)^3 2\omega_k},\quad\omega_k=\sqrt{\mathbf k^2+m^2}.
$$

Hermiticity pairs the two coefficients as adjoints. The field commutators are equivalent to

$$
[a(\mathbf k),a^\dagger(\mathbf q)]=(2\pi)^3 2\omega_k\delta^{(3)}(\mathbf k-\mathbf q),\qquad[a,a]=[a^\dagger,a^\dagger]=0.
$$

For example, inserting the expansion in $[\phi,\dot\phi]$ yields two equal Fourier integrals, each with coefficient $i/2$, and hence $i\delta^{(3)}$. The vacuum obeys $a(\mathbf k)|0\rangle=0$, and repeated [creation operators](../../../../creation-operator.md) generate the symmetric bosonic [Fock space](../../../../fock-space.md). [Normal ordering](../../../../normal-ordering.md) of the quadratic [Hamiltonian](../../../../hamiltonian.md) removes its vacuum constant and gives $H=\int d\Pi_k\,\omega_k a^\dagger a$; the same computation for the spatial [momentum](../../../../momentum-split.md) gives the stipulated [four-momentum](../../../../four-momentum.md) $P^\mu=\int d\Pi_k\,k^\mu a^\dagger a$.

The oscillator algebra now implies

$$
[P^\mu,a(\mathbf k)]=-k^\mu a(\mathbf k),\qquad[P^\mu,a^\dagger(\mathbf k)]=k^\mu a^\dagger(\mathbf k).
$$

Consequently

$$
\begin{aligned}
[P^\mu,\phi(x)]&=\int d\Pi_k\,[-k^\mu a(\mathbf k)e^{-ikx}+k^\mu a^\dagger(\mathbf k)e^{ikx}]\\
&=\boxed{-i\partial^\mu\phi(x)}.
\end{aligned}
$$

Indeed, $\partial^\mu e^{\mp ikx}=\mp ik^\mu e^{\mp ikx}$. For $\mu=0$, the result is $[H,\phi]=-i\dot\phi$, which is the [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md) with the correct sign. As usual, the field identities are interpreted after smearing the operator-valued distributions, or on a suitable common finite-particle domain.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
