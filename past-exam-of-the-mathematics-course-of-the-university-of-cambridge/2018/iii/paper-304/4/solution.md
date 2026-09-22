<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Grassmann field](../../../../../grassmann-field.md) $c$ is odd and the [adjoint scalar field](../../../../../adjoint-scalar-field.md) $\phi$ is even. The two printed signs are consistent with a [right-acting BRST differential](../../../../../right-acting-brst-differential.md), whose [graded Leibniz rule](../../../../../graded-leibniz-rule.md) is

$$
Q(XY)=X(QY)+(-1)^{|Y|}(QX)Y.
$$

The bracket between two odd fields is graded, so $[c,c]=2c^2$. Applying this rule to the ordinary [Lie bracket](../../../../../lie-bracket.md) $[c,\phi]=c\phi-\phi c$ gives

$$
Q^2\phi=[Qc,\phi]+[c,Q\phi].
$$

The second bracket here is graded because both its entries are odd. The [graded Jacobi identity](../../../../../graded-jacobi-identity.md) gives $[c,[c,\phi]]=\tfrac12[[c,c],\phi]$. Therefore

$$
\boxed{Q^2\phi=-\frac12[[c,c],\phi]+\frac12[[c,c],\phi]=0.}
$$

**The side of the odd derivation is essential.** With the usual left [graded Leibniz rule](../../../../../graded-leibniz-rule.md) and the same two printed signs, the result would be $-[[c,c],\phi]$, which is generally nonzero. A left-acting convention must reverse one of those signs. All subsequent [BRST symmetry](../../../../../brst-symmetry.md) formulas here use the right-acting convention.

Choose an anti-Hermitian basis $T^a$ with $[T^b,T^c]=f^{abc}T^a$, an invariant positive [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md), and the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) $D_\mu X=\partial_\mu X+[A_\mu,X]$. Couplings are absorbed into this convention; restoring $D_\mu=\partial_\mu+g[A_\mu,\cdot]$ multiplies each ghost [interaction vertex](../../../../../interaction-vertex.md) below by $g$. The associated [BRST charge](../../../../../brst-charge.md) acts as $QA_\mu=-D_\mu c$, $Q\bar c=ih$, and $Qh=0$.

Write $F^a=\partial\cdot A^a+(n\cdot\partial\phi^a)/\sqrt2$. For the [gauge-fixing fermion](../../../../../gauge-fixing-fermion.md) $\Psi=\int\bar c^a(F^a-ih^a/2)$, the right [graded Leibniz rule](../../../../../graded-leibniz-rule.md) gives

$$
Q\Psi=\int d^4x\left[\frac12h^ah^a+ih^aF^a+\bar c^a(QF)^a\right],\qquad
QF=-\partial^\mu D_\mu c-\frac1{\sqrt2}n\cdot\partial[\phi,c].
$$

The [Gaussian functional integral](../../../../../gaussian-functional-integral.md) over the [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) produces the positive [gauge fixing](../../../../../gauge-fixing.md) term $F^aF^a/2$. The ghost operator is $-\partial\cdot D-(n\cdot\partial)\operatorname{ad}_\phi/\sqrt2$.

Now use the canonical free [kinetic terms](../../../../../kinetic-term.md) $F_{\mu\nu}^aF_{\mu\nu}^a/4+(\partial\phi^a)^2/2$. At nonzero momentum in [Euclidean space](../../../../../euclidean-norm.md) $p$, put $\eta=n\cdot p$. The quadratic kernel for $(A_\mu^a,\phi^a)$, per color, is

$$
K(p)=\begin{pmatrix}
p^2\delta_{\mu\nu}&\eta p_\mu/\sqrt2\\
\eta p_\nu/\sqrt2&p^2+\eta^2/2
\end{pmatrix}.
$$

The transverse gauge-field kernel plus the gauge-fixing longitudinal term has become $p^2\delta_{\mu\nu}$. The scalar [quantum field theory propagator](../../../../../propagator.md) is the inverse [Schur complement](../../../../../schur-complement.md), not merely the inverse of the scalar diagonal entry:

$$
K_{\phi\phi}-K_{\phi A}K_{AA}^{-1}K_{A\phi}
=p^2+\frac{\eta^2}{2}-\frac{\eta^2 p^2}{2p^2}=p^2.
$$

Hence the [free adjoint-scalar propagator in scalar-dependent gauge fixing](../../../../../free-adjoint-scalar-propagator-in-scalar-dependent-gauge-fixing.md) is

$$
\boxed{\langle\phi^a(p)\phi^b(-p)\rangle_0=\frac{\delta^{ab}}{p^2}.}
$$

For completeness the mixed [quantum field theory propagator](../../../../../propagator.md) is $\langle A_\mu^a\phi^b\rangle_0=-\delta^{ab}\eta p_\mu/(\sqrt2 p^4)$; ignoring this mixing would give an incorrect scalar answer.

**The scalar propagator is independent of the gauge vector $n$, not of the momentum component parallel to $n$.** For a unit $n$, $p^2=p_\perp^2+p_\parallel^2$, and the free scalar [quantum field theory propagator](../../../../../propagator.md) still depends on $p_\parallel$. Thus the literal momentum-independence clause in the PDF is false for the standard minimally coupled massless scalar action; the cancellation above establishes the natural gauge-vector-independence statement. The usual massless [zero mode in field theory](../../../../../zero-mode-in-field-theory.md) at $p=0$ needs a separate infrared prescription.

Finally, [integration by parts](../../../../../integration-by-parts.md) gives the ghost action in an unambiguous convention:

$$
S_{\mathrm{gh}}=\int d^4x\left[(\partial_\mu\bar c^a)(\partial_\mu c^a)+f^{abc}(\partial_\mu\bar c^a)A_\mu^b c^c+\frac{f^{abc}}{\sqrt2}(n\cdot\partial\bar c^a)\phi^b c^c\right].
$$

Use $e^{ip\cdot x}$ for the [Fourier transform](../../../../../fourier-transform.md) of every field, with all momenta incoming. Let the antighost carry color $a$ and momentum $q$, the boson color $b$ and momentum $k$, and the ghost color $c$ and momentum $p$, so $q+k+p=0$. Expansion of $e^{-S_{\mathrm{gh}}}$ gives the [ghost vertices in scalar-dependent gauge fixing](../../../../../ghost-vertex-in-scalar-dependent-gauge-fixing.md)

$$
\boxed{\bar c^a(q)A_\mu^b(k)c^c(p):\ -i f^{abc}q_\mu,\qquad
\bar c^a(q)\phi^b(k)c^c(p):\ -\frac{i}{\sqrt2}f^{abc}(n\cdot q).}
$$

The free [Faddeev-Popov ghost field](../../../../../faddeev-popov-ghost.md) propagator is $\delta^{ab}/p^2$ and every closed [ghost loop](../../../../../ghost-loop.md) contributes a minus sign. There are no further ghost [interaction vertices](../../../../../interaction-vertex.md) in this gauge. Factors of $i$ and an overall ghost-vertex sign depend on the [Fourier transform](../../../../../fourier-transform.md) and ghost-ordering conventions; the displayed ghost action fixes both here.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
