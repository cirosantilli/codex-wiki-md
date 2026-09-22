<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the stated [two-dimensional N=(2,2) supersymmetry](../../../../../two-dimensional-n-2-2-supersymmetry.md) conventions, define the [supersymmetric covariant derivatives](../../../../../supersymmetric-covariant-derivative.md)

$$
D_\pm=\frac\partial{\partial\theta^\pm}-i\bar\theta^\pm\partial_\pm,
\qquad
\bar D_\pm=-\frac\partial{\partial\bar\theta^\pm}+i\theta^\pm\partial_\pm.
$$

The terms in which a Grassmann derivative hits the explicit Grassmann coordinate cancel the spacetime-derivative terms, while derivatives involving different signs act on independent coordinates. Therefore

$$
\boxed{\{D_+,Q_\pm\}=\{D_+,\bar Q_\pm\}=0}.
$$

The [twisted chiral superfield](../../../../../twisted-chiral-superfield.md) constraints $D_-U=\bar D_+U=0$ are solved by the twisted chiral coordinates

$$
\widetilde y^+=x^+-i\theta^+\bar\theta^+,
\qquad
\widetilde y^-=x^-+i\theta^-\bar\theta^-.
$$

The superfield depends only on $(\widetilde y^\pm;\theta^+,\bar\theta^-)$ and has the finite [Grassmann variable](../../../../../grassmann-variable.md) expansion

$$
\boxed{U=u+\theta^+\chi_++\bar\theta^-\widetilde\chi_-+\theta^+\bar\theta^-G},
$$

where every component on the right is evaluated at $\widetilde y$; numerical $\sqrt2$ factors may be absorbed into the component definitions.

For one [chiral superfield](../../../../../chiral-superfield.md) $\Phi$ and one twisted chiral superfield $U$, the most general local two-derivative supersymmetric action is

$$
\boxed{
\begin{aligned}
S={}&\int d^2x\,d^4\theta\,K(\Phi,\bar\Phi,U,\bar U)\\
&+\left[\int d^2x\,d\theta^+d\theta^-\,W(\Phi)+\mathrm{h.c.}\right]\\
&+\left[\int d^2x\,d\theta^+d\bar\theta^-\,\widetilde W(U)+\mathrm{h.c.}\right].
\end{aligned}}
$$

Here $K$ is real, $W$ is a holomorphic [superpotential](../../../../../superpotential.md), and $\widetilde W$ is a holomorphic [twisted superpotential](../../../../../twisted-superpotential.md). A full superspace integral, a chiral [F-term](../../../../../f-term.md), and a twisted F-term each vary by a spacetime or Berezin total derivative, so all three are supersymmetric.

Choose the [Vector R-symmetry](../../../../../vector-r-symmetry.md) and [Axial R-symmetry](../../../../../axial-r-symmetry.md) conventions

$$
U(1)_V:\quad\theta^\pm\mapsto e^{i\alpha}\theta^\pm,
\qquad
U(1)_A:\quad\theta^+\mapsto e^{i\beta}\theta^+,
\quad\theta^-\mapsto e^{-i\beta}\theta^-,
$$

with conjugate coordinates transforming oppositely, and assign compatible charges to $\Phi$ and $U$. The D-term is invariant when $K$ is neutral, up to a generalized Kähler transformation. The chiral measure has vector R-charge $-2$ and axial charge zero, whereas the twisted chiral measure has axial R-charge $-2$ and vector charge zero. Hence classical invariance requires

$$
\boxed{
U(1)_V:\ R_V(W)=2,\ R_V(\widetilde W)=0;
\qquad
U(1)_A:\ R_A(W)=0,\ R_A(\widetilde W)=2,
}
$$

together with neutrality of $K$. Equivalently, $W$ and $\widetilde W$ must be quasi-homogeneous with these charges; absent suitable charge assignments, the corresponding superpotential breaks that R-symmetry.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
