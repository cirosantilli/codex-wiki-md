<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the displayed version of [light-cone gauge in string theory](../../../../../../light-cone-gauge-in-string-theory.md), the oscillators have $D-2$ transverse components and

$$
N=\sum_{k=1}^{\infty}\boldsymbol\alpha_{-k}\cdot\boldsymbol\alpha_k.
$$

The center-of-mass [Poisson brackets](../../../../../../poisson-bracket.md) remain $\{x^m,p_n\}=\delta^m_n$, and the transverse oscillator [Poisson brackets](../../../../../../poisson-bracket.md) are $\{\alpha_j^a,\alpha_k^b\}=-ij\delta^{ab}\delta_{j+k,0}$. Other independent brackets vanish. With $\hbar=1$, [canonical quantization](../../../../../../canonical-quantization.md) gives the [canonical commutation relations](../../../../../../canonical-commutation-relation.md)

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_j^a,\alpha_k^b]=j\delta^{ab}\delta_{j+k,0},\qquad
(\alpha_k^a)^\dagger=\alpha_{-k}^a.
$$

The oscillator [Fock vacuum](../../../../../../fock-vacuum.md) at [momentum](../../../../../../momentum.md) $p$ is defined by $\alpha_k^a|0;p\rangle=0$ for $k>0$. It is the ground state of one string, rather than the empty spacetime vacuum. Set $a_k^a=\alpha_k^a/\sqrt{k}$ for $k>0$. The [normal ordering](../../../../../../normal-ordering.md) prescription gives the [string level operator](../../../../../../string-level-operator.md)

$$
\widehat N=\sum_{k>0,a}\alpha_{-k}^a\alpha_k^a
=\sum_{k>0,a}k\,(a_k^a)^\dagger a_k^a,\qquad \widehat N|0;p\rangle=0.
$$

A [Fock state](../../../../../../fock-state.md) basis is obtained by applying $\prod_{k,a}((a_k^a)^\dagger)^{n_{ka}}/\sqrt{n_{ka}!}$ to $|0;p\rangle$, with [string level operator](../../../../../../string-level-operator.md) eigenvalue $N=\sum_{k,a}k n_{ka}$. In particular, its level-one states are

$$
\boxed{\alpha_{-1}^a|0;p\rangle,\qquad a=1,\ldots,D-2.}
$$

They transform as the transverse vector of the [little group](../../../../../../little-group.md) rotation subgroup $SO(D-2)$, precisely the [vector-particle polarizations](../../../../../../vector-particle-polarization.md) of a massless vector. A massive vector would instead require $D-1$ [vector-particle polarizations](../../../../../../vector-particle-polarization.md). This conclusion uses a quantization compatible with the [Lorentz group](../../../../../../lorentz-group.md) of the [bosonic string theory](../../../../../../bosonic-string-theory.md).

The classical mass constraint alone has no quantum [zero-point energy](../../../../../../zero-point-energy.md) shift. Its quantum version includes the [normal-ordering constant of a string](../../../../../../normal-ordering-constant-of-a-string.md) $a$:

$$
(p^2+2\pi T(\widehat N-a))|\mathrm{phys}\rangle=0,\qquad
M^2=2\pi T(N-a).
$$

Masslessness at level one fixes $a=1$, so

$$
\boxed{M_1^2=0,\qquad M_0^2=-2\pi T.}
$$

Thus **the ground state is a [tachyon](../../../../../../tachyon.md)**. Without the quantum ordering shift, the displayed classical constraint would give $M_1^2=2\pi T$ and would not support the stated massless interpretation. In the usual transverse vacuum regularization, $a=(D-2)/24$; consistency with $a=1$ also gives the [critical dimension of string theory](../../../../../../critical-dimension-of-string-theory.md) $D=26$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
