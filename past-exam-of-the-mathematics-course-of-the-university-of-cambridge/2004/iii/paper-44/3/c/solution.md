<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With a vacuum annihilated by all $a_{\mathbf p}^s,b_{\mathbf p}^s$, define the [particle and antiparticle occupation operators of a Dirac field](../../../../../../particle-and-antiparticle-occupation-operators-of-a-dirac-field.md)

$$
N_e=\sum_s\int\frac{d^3p}{(2\pi)^3}a_{\mathbf p}^{s\dagger}a_{\mathbf p}^s,\qquad
N_{\bar e}=\sum_s\int\frac{d^3p}{(2\pi)^3}b_{\mathbf p}^{s\dagger}b_{\mathbf p}^s.
$$

Each counts its corresponding occupied modes. The total positive particle count is

$$
\boxed{N_{\rm total}=N_e+N_{\bar e}.}
$$

Commuting it through either creation operator gives $[N_{\rm total},a^\dagger]=a^\dagger$ and $[N_{\rm total},b^\dagger]=b^\dagger$, so both kinds of one-particle states have eigenvalue one. In a normalized discrete mode, $(a^\dagger a)^2=a^\dagger a$ by the anticommutation relations, so its occupation eigenvalues are $0,1$.

For a [Dirac field](../../../../../../dirac-field.md) there is also a distinct conserved signed fermion number. Inserting the mode expansion into the [normal-ordered](../../../../../../normal-ordering.md) local density gives

$$
\boxed{Q_D=\int d^3x:\psi^\dagger\psi:
=N_e-N_{\bar e}.}
$$

Spatial integration makes the same-sector momenta equal. The cross terms vanish by $u^\dagger(\mathbf p)v(-\mathbf p)=0$; [normal ordering](../../../../../../normal-ordering.md) of $bb^\dagger$ supplies the minus sign for the [antiparticles](../../../../../../antiparticle.md). Thus the density integral is not the total positive particle count. It generates the global phase symmetry, and for [Electron](../../../../../../electron.md) charge $-e$ the electric charge is $Q_{\rm em}=-eQ_D$.

The free [normal-ordered](../../../../../../normal-ordering.md) [Hamiltonian](../../../../../../hamiltonian.md) is

$$
H=\sum_s\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}
\left(a_{\mathbf p}^{s\dagger}a_{\mathbf p}^s+
b_{\mathbf p}^{s\dagger}b_{\mathbf p}^s\right),
$$

so $N_e,N_{\bar e},N_{\rm total}$ and $Q_D$ are conserved in the free theory. In an interacting theory, pair creation can change the total count while preserving the signed charge. This distinguishes a positive occupation [number operator](../../../../../../number-operator.md) from the charge behind [Dirac fermion number conservation](../../../../../../dirac-fermion-number-conservation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
