<h1 id="32b/solution">Solution</h1>

↑ **Parent:** [32B](../32b.md)

The [spin raising operator](../../../../../spin-raising-operator.md) and [spin lowering operator](../../../../../spin-lowering-operator.md) are

$$
S_+=S_x+iS_y,
\qquad
S_-=S_x-iS_y.
$$

The [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) imply

$$
[S_z,S_\pm]=\pm\hbar S_\pm,
\qquad
[S^2,S_\pm]=0,
$$

so $S_\pm|s,\sigma\rangle$ is proportional to $|s,\sigma\pm1\rangle$. Since

$$
S_\mp S_\pm=S^2-S_z^2\mp\hbar S_z,
$$

its squared [norm](../../../../../norm.md) is

$$
\begin{aligned}
\|S_\pm|s,\sigma\rangle\|^2
&=\langle s,\sigma|S_\mp S_\pm|s,\sigma\rangle\\
&=\hbar^2\{s(s+1)-\sigma(\sigma\pm1)\}.
\end{aligned}
$$

Choosing the conventional positive phase gives

$$
\boxed{
S_\pm|s,\sigma\rangle
=\hbar\sqrt{s(s+1)-\sigma(\sigma\pm1)}
\,|s,\sigma\pm1\rangle.}
$$

Using the [spin ladder operators](../../../../../spin-ladder-operator.md),

$$
\mathbf S^{(1)}\mathbin\cdot\mathbf S^{(2)}
=S_z^{(1)}S_z^{(2)}
+\frac12\left(S_+^{(1)}S_-^{(2)}
+S_-^{(1)}S_+^{(2)}\right),
$$

and therefore

$$
H=\alpha S_z^{(1)}S_z^{(2)}
+\frac\alpha2\left(S_+^{(1)}S_-^{(2)}
+S_-^{(1)}S_+^{(2)}\right)
+B\left(S_z^{(1)}-S_z^{(2)}\right).
$$

In the ordered product basis of the [tensor product of quantum systems](../../../../../tensor-product-of-quantum-systems.md)

$$
|\uparrow\uparrow\rangle,\quad
|\uparrow\downarrow\rangle,\quad
|\downarrow\uparrow\rangle,\quad
|\downarrow\downarrow\rangle,
$$

the [matrix representation](../../../../../matrix-representation.md) is

$$
H=
\begin{pmatrix}
\alpha\hbar^2/4&0&0&0\\
0&-\alpha\hbar^2/4+B\hbar&\alpha\hbar^2/2&0\\
0&\alpha\hbar^2/2&-\alpha\hbar^2/4-B\hbar&0\\
0&0&0&\alpha\hbar^2/4
\end{pmatrix}.
$$

The two parallel-spin states are already [eigenvectors](../../../../../eigenvector.md). Diagonalizing the central block gives the four [energy eigenvalues](../../../../../energy-eigenvalue.md)

$$
\boxed{
E_{\uparrow\uparrow}=E_{\downarrow\downarrow}
=\frac{\alpha\hbar^2}{4},
\qquad
E_\pm=-\frac{\alpha\hbar^2}{4}
\pm\sqrt{B^2\hbar^2+\frac{\alpha^2\hbar^4}{4}}.}
$$

This is the spectrum of the [Two-spin Heisenberg Hamiltonian in an opposing longitudinal field](../../../../../two-spin-heisenberg-hamiltonian-in-an-opposing-longitudinal-field.md).

The asserted ground-state ordering requires the antiferromagnetic case $\alpha>0$. As $B\to0$,

$$
E_-=-\frac{3\alpha\hbar^2}{4},
\qquad
E_+=E_{\uparrow\uparrow}=E_{\downarrow\downarrow}
=\frac{\alpha\hbar^2}{4}.
$$

The corresponding state at $E_-$ is the unique [spin-one-half singlet state](../../../../../spin-one-half-singlet-state.md)

$$
|0,0\rangle
=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2},
$$

whereas the three states at the first excited energy form the [spin-one-half triplet state](../../../../../spin-one-half-triplet-state.md).

Indeed, for the [total angular momentum operator](../../../../../total-angular-momentum-operator.md)

$$
\mathbf S=\mathbf S^{(1)}+\mathbf S^{(2)},
$$

one has at $B=0$

$$
H=\frac\alpha2\left(
S^2-(S^{(1)})^2-(S^{(2)})^2
\right).
$$

The Hamiltonian then has [rotational symmetry](../../../../../rotational-symmetry.md), so energy depends only on the [total-spin sector](../../../../../total-spin-sector.md). The singlet has total spin $s=0$ and multiplicity one; the triplet has $s=1$ and multiplicity $2s+1=3$. This rotational symmetry explains why the triplet [energy eigenspace](../../../../../energy-eigenspace.md) has dimension three.

## ↑ Ancestors (10)

1. [32B](../32b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
