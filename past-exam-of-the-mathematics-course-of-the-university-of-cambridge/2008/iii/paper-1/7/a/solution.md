<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the involution as the adjoint for the Hilbert-space structure on $V$. The hypotheses make $\Omega$ a [cyclic vector for an operator algebra](../../../../../../cyclic-vector-for-an-operator-algebra.md) for both $A$ and $A'$. They also make it a [separating vector](../../../../../../separating-vector-for-an-operator-algebra.md) for each: if $a\Omega=0$, then $a$ vanishes on $A'\Omega=V$, and similarly for $A'$. Thus the [Tomita operator](../../../../../../tomita-operator.md)

$$
S(a\Omega)=a^*\Omega
$$

is well defined, antilinear, invertible and satisfies $S^2=I$. Define the [modular operator](../../../../../../modular-operator.md) and [modular conjugation](../../../../../../modular-conjugation.md) by

$$
\boxed{\Delta=S^*S,\qquad J=S\Delta^{-1/2},\qquad S=J\Delta^{1/2}.}
$$

We calculate them explicitly to prove the commutant assertion.

The finite-dimensional structure of a [unital](../../../../../../unital-algebra.md) [star-algebra](../../../../../../star-algebra.md) gives an orthogonal decomposition

$$
V=\bigoplus_j(\mathbb C^{n_j}\otimes\mathbb C^{m_j}),\qquad
A=\bigoplus_j(M_{n_j}(\mathbb C)\otimes I_{m_j}),\qquad
A'=\bigoplus_j(I_{n_j}\otimes M_{m_j}(\mathbb C)).
$$

This is the usual matrix-block structure: minimal central [projections](../../../../../../projection-linear-algebra.md) separate the simple summands, and each simple [matrix algebra](../../../../../../matrix-algebra.md) acts as its defining representation with a multiplicity space. Identify each [vector](../../../../../../vector.md) block with an $n_j$-by-$m_j$ [matrix](../../../../../../matrix.md) $D_j$ with its [Hilbert-Schmidt](../../../../../../hilbert-schmidt-operator.md) [inner product](../../../../../../inner-product.md). The two algebras act by left and right multiplication. If $D_j$ has rank $r_j$, the left orbit has dimension $n_jr_j$ and the right orbit dimension $m_jr_j$. Cyclicity on both sides therefore forces $r_j=m_j=n_j$. Every $D_j$ is square and invertible.

Right multiplication by a suitable unitary is a unitary change of this identification commuting with the left algebra. The polar decomposition of each $D_j$ therefore lets us assume $D_j>0$. In one such block, for an arbitrary [matrix](../../../../../../matrix.md) $X=aD$, the [Tomita operator](../../../../../../tomita-operator.md) is

$$
S(X)=D^{-1}X^*D.
$$

Its polar factors are

$$
\boxed{J(X)=X^*,\qquad \Delta^{1/2}(X)=DXD^{-1},\qquad
\Delta(X)=D^2XD^{-2}.}
$$

Indeed, $J$ is an antiunitary involution and $J\Delta^{1/2}(X)=D^{-1}X^*D$. The fact that $\Delta^{1/2}$ is a [positive operator](../../../../../../positive-operator.md) is transparent in a [basis](../../../../../../basis.md) diagonalizing $D$: it multiplies the [matrix](../../../../../../matrix.md) unit $E_{kl}$ by the positive ratio $d_k/d_l$. These are therefore the unique polar factors of $S$.

Finally, if $L_a$ denotes left multiplication,

$$
(JL_aJ)(X)=(aX^*)^*=Xa^*.
$$

As $a$ ranges over the full [matrix](../../../../../../matrix.md) block, these are exactly its right multiplications. Applying this on every block and transporting back by the unitary identifications proves

$$
\boxed{JAJ=A'.}
$$

This also establishes the required modular definitions intrinsically, independent of the chosen [matrix](../../../../../../matrix.md) coordinates.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
