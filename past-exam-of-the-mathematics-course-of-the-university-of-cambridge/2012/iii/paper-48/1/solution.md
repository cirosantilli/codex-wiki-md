<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $\hbar=1$ and let $N=2I\in\mathbb Z_{\geq0}$. A concrete [irreducible spin representation](../../../../../irreducible-spin-representation.md) is the [symmetric power](../../../../../symmetric-power.md)

$$
\mathcal H_I=\operatorname{Sym}^{N}\mathbb C^2.
$$

Start with $N$ copies of the defining [SU(2)](../../../../../su-2-group.md) doublet and restrict their [tensor product representation](../../../../../tensor-product-of-group-representations.md) to the completely symmetric subspace. Its orthonormal basis consists of symmetric states with $I+m$ up components and $I-m$ down components, where $m=I,I-1,\ldots,-I$. There are $N+1=2I+1$ such states. The total generators are $J_i=\sum_{a=1}^N\sigma_i^{(a)}/2$, acting on this subspace, where $\sigma_i$ are the [Pauli matrices](../../../../../pauli-matrices.md). This also constructs the trivial representation when $I=0$.

The [spin ladder operators](../../../../../spin-ladder-operator.md) $J_\pm=J_1\pm iJ_2$ satisfy

$$
[J_3,J_\pm]=\pm J_\pm,\qquad [J_+,J_-]=2J_3.
$$

The [Casimir operator](../../../../../casimir-element.md) $J^2=\sum_iJ_i^2$ commutes with every generator. On the [highest-weight vector](../../../../../highest-weight-vector.md) $|I,I\rangle$, the identity $J^2=J_-J_++J_3(J_3+1)$ gives its [eigenvalue](../../../../../eigenvalue.md) $I(I+1)$. With phases chosen to make the lowering coefficients positive,

$$
\boxed{J_-|I,m\rangle=\sqrt{(I+m)(I-m+1)}\,|I,m-1\rangle,}
$$



$$
J_+|I,m\rangle=\sqrt{(I-m)(I+m+1)}\,|I,m+1\rangle.
$$

The squared [norm](../../../../../norm.md) of the lowered state follows from $J_+J_-=J^2-J_3(J_3-1)$. The ladder stops exactly at $m=-I$. Every weight is connected to every other by these operators, and $J_3$ has distinct [eigenvalues](../../../../../eigenvalue.md). Hence any [invariant subspace](../../../../../invariant-subspace.md) contains a weight vector and then the whole ladder: the representation is irreducible.

For $k=I-m$, successive lowering has squared [norm](../../../../../norm.md)

$$
\prod_{r=0}^{k-1}(2I-r)(r+1)=\frac{(2I)!k!}{(2I-k)!}.
$$

Thus the [normalized highest-weight lowering formula](../../../../../normalized-highest-weight-lowering-formula.md) is

$$
\boxed{|I,m\rangle=\sqrt{\frac{(I+m)!}{(2I)!(I-m)!}}\,(J_-)^{I-m}|I,I\rangle.}
$$

All factorial arguments are nonnegative integers, including for half-integral $I$.

The [unitary representation](../../../../../unitary-representation.md) of an [isospin rotation](../../../../../isorotation.md) is

$$
\boxed{U[R(\theta,\mathbf n)]=e^{-i\theta\mathbf n\cdot\mathbf J}.}
$$

Its [matrix](../../../../../matrix.md) in the weight basis is $D^{(I)}_{m'm}(R)=\langle I,m'|U[R]|I,m\rangle$. Insert the completeness relation between two operators to obtain

$$
D^{(I)}(g_1g_2)=D^{(I)}(g_1)D^{(I)}(g_2),\quad
D^{(I)}(1)=I,\quad D^{(I)}(g^{-1})=D^{(I)}(g)^\dagger.
$$

These verify the [group representation](../../../../../group-representation.md) and unitarity properties, and the ladder argument gives irreducibility. Here rotations carry their [SU(2)](../../../../../su-2-group.md) lifts: $U(2\pi)=(-1)^{2I}I$. Integer $I$ descends to the ordinary [SO(3) group](../../../../../so-3-group.md); half-integral $I$ is a representation of its double cover, not a single-valued representation of $SO(3)$.

For $I=1$, order the basis as $(|1,1\rangle,|1,0\rangle,|1,-1\rangle)$. The lowering and raising coefficients give the [spin-one half-turn matrix](../../../../../spin-one-half-turn-matrix.md)

$$
J_2^{(1)}=\frac1{\sqrt2}\begin{pmatrix}0&-i&0\\i&0&-i\\0&i&0\end{pmatrix},\qquad
(J_2^{(1)})^2=\frac12\begin{pmatrix}1&0&-1\\0&2&0\\-1&0&1\end{pmatrix}.
$$

Multiplication shows $(J_2^{(1)})^3=J_2^{(1)}$. Reduce the [matrix exponential](../../../../../matrix-exponential.md) using this identity:

$$
e^{-i\theta J_2}=I-i\sin\theta\,J_2+(\cos\theta-1)J_2^2.
$$

At $\theta=\pi$ it becomes

$$
\boxed{e^{-i\pi J_2}=\begin{pmatrix}0&0&1\\0&-1&0\\1&0&0\end{pmatrix},\qquad
e^{-i\pi J_2}|1,m\rangle=-(-1)^m|1,-m\rangle.}
$$

Thus its [matrix](../../../../../matrix.md) elements are $-(-1)^m\delta_{m',-m}$. In the [pion](../../../../../pion.md) phases $|\pi^\pm\rangle=|1,\pm1\rangle$, $|\pi^0\rangle=|1,0\rangle$, this [isospin rotation](../../../../../isorotation.md) exchanges the two charged states with positive coefficients and negates the neutral state.

[Charge conjugation](../../../../../charge-conjugation.md) is linear and unitary here. Similarity preserves [commutators](../../../../../commutator.md), so

$$
[\mathcal CJ_i\mathcal C^{-1},\mathcal CJ_j\mathcal C^{-1}]
=\mathcal C[J_i,J_j]\mathcal C^{-1}
=i\epsilon_{ijk}\mathcal CJ_k\mathcal C^{-1}.
$$

Consequently the conjugated generators obey the same [Lie algebra](../../../../../lie-algebra-split.md). The specified signs also give $\mathcal CJ_\pm\mathcal C^{-1}=-J_\mp$. Since $|\pi^\pm\rangle=J_\pm|\pi^0\rangle/\sqrt2$ and the neutral state has positive [charge conjugation](../../../../../charge-conjugation.md) [eigenvalue](../../../../../eigenvalue.md),

$$
\boxed{\mathcal C|\pi^\pm\rangle=-|\pi^\mp\rangle.}
$$

The signs depend on the chosen charged-state phases, which have been fixed by the ladder convention.

Conjugation by $R_\pi=e^{-i\pi J_2}$ changes $(J_1,J_2,J_3)$ to $(-J_1,J_2,-J_3)$, exactly as [charge conjugation](../../../../../charge-conjugation.md) does. Their product, the [G parity](../../../../../g-parity.md) operator, therefore satisfies

$$
GJ_iG^{-1}=\mathcal C(R_\pi J_iR_\pi^{-1})\mathcal C^{-1}=J_i.
$$

The [Schur lemma](../../../../../schur-s-lemma.md) makes $G$ scalar on each irreducible [isospin](../../../../../isospin.md) multiplet, hence independent of $m$. On the neutral [pion](../../../../../pion.md), $G|\pi^0\rangle=-\mathcal C|\pi^0\rangle=-|\pi^0\rangle$. Therefore the [pion G-parity](../../../../../pion-g-parity.md) is

$$
\boxed{G=-1\quad\text{on all three pion states}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
