<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix a positive-mass [unitary irreducible representation](../../../../../unitary-irreducible-representation.md) at rest, $P^\mu=(M,0,0,0)$ with $M>0$. Use the [central charge in supersymmetry](../../../../../central-charge-in-supersymmetry.md) convention

$$
\{Q^A_\alpha,\bar Q_{\dot\beta B}\}=2\delta^A_B\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad\{Q^A_\alpha,Q^B_\beta\}=\epsilon_{\alpha\beta}Z^{AB},\qquad Z^{AB}=-Z^{BA},
$$

The conjugate relation is $\{\bar Q_{\dot\alpha A},\bar Q_{\dot\beta B}\}=\epsilon_{\dot\alpha\dot\beta}\overline{Z^{AB}}$, with the dotted epsilon tensor the conjugate of the undotted one. The [supercharges](../../../../../supersymmetry-generator.md) commute with $P_\mu$ and the central charges. Their Lorentz transformation is that of a [Weyl spinor](../../../../../weyl-spinor.md); together with the ordinary [Poincare algebra](../../../../../poincare-algebra.md), these relations specify the [Super-Poincaré algebra](../../../../../super-poincare-algebra.md). Take $\epsilon_{12}=1$ and write $Z^{12}=2z$. This makes the normalization of the mass bound explicit: a convention that writes $2\epsilon_{\alpha\beta}Z^{AB}$ instead has $z=Z^{12}$.

When $Z=0$, define four [fermionic annihilation operators](../../../../../fermionic-annihilation-operator.md) and their [fermionic creation operators](../../../../../fermionic-creation-operator.md) by

$$
a^A_\alpha=\frac{Q^A_\alpha}{\sqrt{2M}},\qquad(a^A_\alpha)^\dagger=\frac{\bar Q_{\dot\alpha A}}{\sqrt{2M}}.
$$

In the rest frame they obey the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) $\{a_i,a_j^\dagger\}=\delta_{ij}$ and $\{a_i,a_j\}=0$. Choose a spin-zero [Clifford vacuum](../../../../../clifford-vacuum.md) annihilated by all four $a_i$. Acting with each distinct creator at most once constructs the [fermionic Fock space](../../../../../fermionic-fock-space.md)

$$
a_{i_1}^\dagger\cdots a_{i_k}^\dagger|\Omega\rangle,\qquad i_1<\cdots<i_k,\qquad k=0,1,2,3,4.
$$

The five levels have the [binomial coefficient](../../../../../binomial-coefficient.md) multiplicities $1,4,6,4,1$, so the [massive supermultiplet](../../../../../massive-supermultiplet.md) contains $2^4=16$ states. The four creators are two copies of the spin-one-half [SU(2) representation](../../../../../representation-theory-of-su-2.md). Their second [exterior power](../../../../../exterior-power.md) is

$$
\bigwedge^2(\mathbf2\otimes\mathbf2)=\bigl(\operatorname{Sym}^2\mathbf2\otimes\bigwedge^2\mathbf2\bigr)\oplus\bigl(\bigwedge^2\mathbf2\otimes\operatorname{Sym}^2\mathbf2\bigr).
$$

Here the first factor carries physical spin and the second counts the two supersymmetries. Thus level two contains one spin-one triplet and three spin-zero singlets; levels one and three each contain two spin-one-half doublets. The final spin content is

$$
\boxed{5\text{ spin-0 states}+4\text{ spin-}\tfrac12\text{ doublets}+1\text{ spin-1 triplet}=16\text{ states}.}
$$

Even levels give eight [boson](../../../../../boson.md) states and odd levels eight [fermion](../../../../../fermion.md) states, exhibiting [boson-fermion degeneracy in a supermultiplet](../../../../../boson-fermion-degeneracy-in-a-supermultiplet.md).

For nonzero $z=|z|e^{i\varphi}$, pair the two supersymmetries before normalizing. Define

$$
q_\alpha=Q^1_\alpha,\qquad r_\alpha=\epsilon_{\alpha\beta}(Q^2_\beta)^\dagger,\qquad b^\pm_\alpha=\frac{q_\alpha\pm e^{i\varphi}r_\alpha}{\sqrt2}.
$$

The rest-frame algebra gives $\{q_\alpha,r_\beta^\dagger\}=2z\delta_{\alpha\beta}$ and consequently

$$
\{b^\pm_\alpha,(b^\pm_\beta)^\dagger\}=2(M\pm|z|)\delta_{\alpha\beta},\qquad\{b^+_\alpha,(b^-_\beta)^\dagger\}=0.
$$

For $M>|z|$, divide $b^\pm$ by $\sqrt{2(M\pm|z|)}$ to recover four normalized oscillators. Positivity of the [Hilbert space](../../../../../hilbert-space-split.md) [norm](../../../../../norm.md) proves the [BPS bound in supersymmetry](../../../../../bps-bound-in-supersymmetry.md), since

$$
\|b^-_\alpha|v\rangle\|^2+\|(b^-_\alpha)^\dagger|v\rangle\|^2=2(M-|z|)\|v\|^2\ge0.
$$

Therefore

$$
\boxed{M\ge |z|=\tfrac12|Z^{12}|.}
$$

For a [BPS state](../../../../../bps-state.md) saturating this bound, both $b^-_\alpha$ and their adjoints annihilate every state of the representation. Four of the eight real [supercharges](../../../../../supersymmetry-generator.md) act trivially. Only the two $b^+$ oscillators remain, so a scalar [Clifford vacuum](../../../../../clifford-vacuum.md) gives a [shortened massive supermultiplet](../../../../../shortened-massive-supermultiplet.md) with two spin-zero states and one spin-one-half doublet:

$$
\boxed{M=|z|:\quad 4\text{ states}=2\text{ bosons}+2\text{ fermions},\quad\text{one-half of the supersymmetry preserved}.}
$$

This is the irreducible count at fixed central charge. A [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) can require the charge-conjugate multiplet as well, doubling it to eight states; the full [hypermultiplet](../../../../../hypermultiplet.md) count must not be confused with this four-state count. Saturation is a representation-theoretic relation between mass and conserved charge: shortening persists while the state remains BPS, although its existence can change across parameter space.

For even $\mathcal N=2n$, [unitary skew-diagonalization of an antisymmetric matrix](../../../../../unitary-skew-diagonalization-of-an-antisymmetric-matrix.md) brings the central-charge [matrix](../../../../../matrix.md) to blocks $2z_r\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, $r=1,\ldots,n$. Repeat the oscillator construction separately for each block. Every block supplies two oscillators with [norm](../../../../../norm.md) $2(M+|z_r|)$ and two with [norm](../../../../../norm.md) $2(M-|z_r|)$, giving

$$
\boxed{M\ge\max_r|z_r|.}
$$

If $k$ blocks saturate, $2k$ complex oscillators disappear, leaving $2\mathcal N-2k$. Starting with spin $j_0$, the irreducible state count and preserved fraction are

$$
\boxed{\dim\mathcal H=(2j_0+1)2^{\,2\mathcal N-2k},\qquad\frac{\text{preserved real supercharges}}{4\mathcal N}=\frac{k}{\mathcal N}.}
$$

The largest massive shortening, $k=n$, preserves one-half. The ordinary massive representation has $k=0$. This rest-frame discussion excludes $M=0$, where the [massless supermultiplet](../../../../../massless-supermultiplet.md) construction uses a null momentum instead.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
