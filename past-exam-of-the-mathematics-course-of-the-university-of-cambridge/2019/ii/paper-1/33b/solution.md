<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are $[X_i,X_j]=[P_i,P_j]=0$ and $[X_i,P_j]=i\hbar\delta_{ij}$. Substitution into the definitions of the [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) gives

$$
\boxed{[A_i^\dagger,A_j^\dagger]=0,\qquad[A_i,A_j]=0,\qquad[A_i,A_j^\dagger]=\delta_{ij}.}
$$

The normalized [ground state](../../../../../ground-state.md) is defined by

$$
A_i|0\rangle=0\quad(i=1,2,3),
\qquad \langle0|0\rangle=1.
$$

Repeated use of $[A_i,A_i^\dagger]=1$ gives the [Cartesian number state of the three-dimensional isotropic harmonic oscillator](../../../../../cartesian-number-state-of-the-three-dimensional-isotropic-harmonic-oscillator.md)

$$
\boxed{|n_1,n_2,n_3\rangle
=\frac{(A_1^\dagger)^{n_1}(A_2^\dagger)^{n_2}(A_3^\dagger)^{n_3}}
{\sqrt{n_1!n_2!n_3!}}|0\rangle,}
$$

with [energy eigenvalue](../../../../../energy-eigenvalue.md)

$$
E_{n_1n_2n_3}=\hbar\omega\left(n_1+n_2+n_3+\frac32\right).
$$

Inverting the ladder-operator definitions yields

$$
X_i=\sqrt{\frac{\hbar}{2\mu\omega}}(A_i+A_i^\dagger),
\qquad
P_i=i\sqrt{\frac{\mu\hbar\omega}{2}}(A_i^\dagger-A_i).
$$

The antisymmetry of the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) then cancels the two-creation and two-annihilation terms in $\mathbf L=\mathbf X\times\mathbf P$, leaving the [orbital angular momentum in oscillator ladder operators](../../../../../orbital-angular-momentum-in-oscillator-ladder-operators.md)

$$
\boxed{L_i=-i\hbar\varepsilon_{ijk}A_j^\dagger A_k.}
$$

Write $|j\rangle=A_j^\dagger|0\rangle$. Then

$$
L_i|j\rangle=-i\hbar\varepsilon_{ikj}|k\rangle,
\qquad
L^2|j\rangle=2\hbar^2|j\rangle.
$$

Since the [orbital angular momentum](../../../../../orbital-angular-momentum.md) eigenvalue is $\ell(\ell+1)\hbar^2$, every first-excited state has

$$
\boxed{\ell=1.}
$$

Finally,

$$
L_z|x\rangle=i\hbar|y\rangle,
\qquad
L_z|y\rangle=-i\hbar|x\rangle.
$$

Therefore the normalized [magnetic quantum number](../../../../../magnetic-quantum-number.md) $m=+1$ state can be chosen as

$$
\boxed{|\psi\rangle=\frac{|x\rangle+i|y\rangle}{\sqrt2}
=\frac{A_x^\dagger+iA_y^\dagger}{\sqrt2}|0\rangle,}
$$

which obeys $L_z|\psi\rangle=\hbar|\psi\rangle$ and $\lVert|\psi\rangle\rVert=1$.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
