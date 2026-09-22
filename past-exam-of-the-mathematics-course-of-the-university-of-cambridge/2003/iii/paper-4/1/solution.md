<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Here is [Witt's lemma](../../../../../witt-s-theorem.md) with the hypotheses appropriate to the [classical groups](../../../../../classical-group.md). Let $V$ be finite-dimensional with a nonsingular [alternating bilinear form](../../../../../alternating-bilinear-form.md), a nonsingular [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) in [characteristic](../../../../../characteristic-of-a-field.md) different from two, or a nonsingular [Hermitian form](../../../../../hermitian-form.md) with nontrivial involution. Every [isometry of a space with a form](../../../../../isometry-of-a-space-with-a-form.md) $\phi:U\to U'$ between [vector subspaces](../../../../../vector-subspace.md) extends to a form-preserving [automorphism](../../../../../automorphism.md) of $V$. For [quadratic forms](../../../../../quadratic-form.md), the same statement holds in every [characteristic](../../../../../characteristic-of-a-field.md) when the [polar bilinear form of a quadratic form](../../../../../polar-bilinear-form-of-a-quadratic-form.md) is nonsingular and the [isometry of a space with a form](../../../../../isometry-of-a-space-with-a-form.md) preserves the [quadratic form](../../../../../quadratic-form.md) itself. **The restricted forms on $U,U'$ may be degenerate.** We prove these versions, including the characteristic-two quadratic case needed later.

For an [alternating bilinear form](../../../../../alternating-bilinear-form.md) $B$, split the restricted space as $U=H\oplus R$, where $R=U\cap U^\perp$ and $B|_H$ is nonsingular. Choose a [symplectic basis](../../../../../symplectic-basis.md) for $H$ and a [basis](../../../../../basis.md) $r_1,\ldots,r_t$ of $R$. The [nondegenerate](../../../../../nondegenerate-bilinear-form.md) form on $V$ supplies vectors $s_j$ in $H^\perp$ with $B(r_i,s_j)=\delta_{ij}$. Adding linear combinations of the $r_i$ to the $s_j$ makes $B(s_i,s_j)=0$: for each pair $i<j$ one may cancel its pairing by adding an appropriate multiple of $r_i$ to $s_j$, without disturbing the dual pairings or previously treated pairs. This uses no division by two. Thus $H$ together with the pairs $(r_i,s_i)$ is nonsingular and its [orthogonal complement for a sesquilinear form](../../../../../orthogonal-complement-for-a-sesquilinear-form.md) has a [symplectic basis](../../../../../symplectic-basis.md).

Apply the same construction to $\phi(H),\phi(r_i)$, choosing partners $s_i'$ there. The two completed [bases](../../../../../basis.md) have identical alternating [Gram matrices](../../../../../gram-matrix.md) and equal remaining [dimensions](../../../../../dimension-vector-space.md). The [linear map](../../../../../linear-map.md) matching these [bases](../../../../../basis.md) preserves $B$ and agrees with $\phi$ on $H\oplus R=U$. This proves the alternating version over an arbitrary [field](../../../../../field.md), including [characteristic](../../../../../characteristic-of-a-field.md) two.

For a [quadratic form](../../../../../quadratic-form.md) $Q$, define its [polar bilinear form of a quadratic form](../../../../../polar-bilinear-form-of-a-quadratic-form.md) by $B(x,y)=Q(x+y)-Q(x)-Q(y)$. Its symmetry

$$
s_a(x)=x-\frac{B(x,a)}{Q(a)}a\qquad(Q(a)\ne0)
$$

preserves $Q$. The zero-dimensional case is immediate. Induct on $\dim U$: choose $Q(t)\ne0$ and a [hyperplane](../../../../../hyperplane.md) $K\subseteq U\cap t^\perp$. Extending $\phi|_K$ first reduces to $\phi|_K=I$. Put $U=K\oplus Fu$, $v=\phi(u)$, $d=u-v\in S=K^\perp$. If $Q(d)\ne0$, $s_d$ completes the extension. Otherwise $B(u,d)=B(v,d)=0$. The [hyperplanes](../../../../../hyperplane.md) $H=S\cap u^\perp$, $H'=S\cap v^\perp$ are proper because $S^\perp=K$.

For $a\in S\setminus(H\cup H')$ with $Q(a)\ne0$, set $c=u-s_a(v)$. Then

$$
Q(c)=\frac{B(u,a)B(v,a)}{Q(a)}\ne0,
$$

and $s_as_c$ fixes $K$ and sends $u$ to $v$. If no such $a$ exists and $|F|>2$, the identity

$$
0=Q(a+\lambda z)=\lambda^2Q(z)+\lambda B(a,z),\qquad z\in H\cap H',\quad\lambda\in F
$$

forces $Q(z)=B(a,z)=0$. The complement of two [hyperplanes](../../../../../hyperplane.md) spans $S$: adding a multiple of any outside vector avoids at most two forbidden scalars. Hence $d\perp S$, so $H=H'$, forcing $Q|_S=0$, contrary to $t\in S$.

Over $\mathbb F_2$, choose $a$ outside both [hyperplanes](../../../../../hyperplane.md). In the remaining case $Q(a)=Q(d)=B(a,d)=0$, and $B(a,u)=B(a,v)=1$. The explicit map

$$
g(x)=x+B(d,x)a+B(a,x)d
$$

has $g^2=I$, preserves $Q$ by cancellation of its two cross terms, fixes $K$ and sends $u$ to $v$. This closes the induction. The characteristic-independent symmetry argument and its binary exceptional step are also treated in [Casselman's quadratic-form notes](https://www.math.ubc.ca/~cass/research/pdf/QForms.pdf) and [Elman, Karpenko and Merkurjev, section 8](https://www.math.ucla.edu/~rse/book/Kniga.pdf).

In odd [characteristic](../../../../../characteristic-of-a-field.md) a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) is recovered by the [polarization identity](../../../../../polarization-identity.md) for $Q(x)=B(x,x)/2$, so the quadratic proof also proves its extension theorem. For completeness, the [Hermitian form](../../../../../hermitian-form.md) case has a similarly explicit induction. Take $h$ linear in the first variable, with conjugation $a\mapsto\bar a$. For [anisotropic vectors for a form](../../../../../anisotropic-vector-for-a-form.md) $u,v$ with equal value $A=h(u,u)=h(v,v)\ne0$, let $d=u-v$ and $c=h(u,d)$. When $c\ne0$, the rank-one map

$$
g(x)=x-\frac{h(x,d)}c\,d
$$

sends $u$ to $v$ and preserves $h$, since $h(d,d)=c+\bar c$ and the extra coefficient in $h(gx,gy)$ is

$$
-\frac1c-\frac1{\bar c}+\frac{c+\bar c}{c\bar c}=0.
$$

When $c=0$, insert $\lambda u$ with $\lambda\bar\lambda=1$, $\lambda\ne1$, and use two such maps. Such a scalar exists for a nontrivial involution: $\lambda=a/\bar a$ with $a\ne\bar a$ works. If the source [vector subspace](../../../../../vector-subspace.md) contains an [anisotropic vector for a form](../../../../../anisotropic-vector-for-a-form.md), align it this way and induct in its nonsingular [orthogonal complement for a sesquilinear form](../../../../../orthogonal-complement-for-a-sesquilinear-form.md).

If instead every source vector is isotropic, the Hermitian [polarization identity](../../../../../polarization-identity.md) makes its whole restricted form zero. Choose $e$ in its [basis](../../../../../basis.md) and a partner $f$ pairing to one with $e$ and to zero with the remaining source [basis](../../../../../basis.md). Make $h(f,f)=0$ by replacing $f$ by $f-te$, where $t+\bar t=h(f,f)$. The trace map is onto the fixed [field](../../../../../field.md): in odd [characteristic](../../../../../characteristic-of-a-field.md) divide by two; in [characteristic](../../../../../characteristic-of-a-field.md) two scale a nonzero trace. Choose $a+\bar a\ne0$. The orthogonal vectors $e+af$ and $e-\bar af$ have nonzero values $a+\bar a$ and its negative, so the preceding rank-one construction aligns this entire [hyperbolic pair](../../../../../hyperbolic-pair.md) with its target pair. The remaining source [basis](../../../../../basis.md) lies in the pair's [orthogonal complement for a sesquilinear form](../../../../../orthogonal-complement-for-a-sesquilinear-form.md); induction finishes the Hermitian proof.

The hypotheses matter. For example, the identity-matrix [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) on $\mathbb F_2^3$ has canonical vector $c=(1,1,1)$ characterized by $B(x,c)=B(x,x)$, so every [isometry of a space with a form](../../../../../isometry-of-a-space-with-a-form.md) fixes $c$. The one-dimensional map $e_1\mapsto c$ preserves the restricted [bilinear form](../../../../../bilinear-form.md) but cannot extend. Thus “all symmetric forms in [characteristic](../../../../../characteristic-of-a-field.md) two” is not a correct replacement for the quadratic or alternating versions proved above.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
