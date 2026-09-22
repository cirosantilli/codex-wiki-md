<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite point $p$, use the [valuation](../../../../../../valuation.md) $v_p$ with local parameter $u=t-p$; at infinity use $u=1/t$. Its extensions $w$ to $E$ are permuted transitively by $G$. The completed residue [field](../../../../../../field.md) is $F$, because $F$ is algebraically closed, so the local [decomposition group](../../../../../../decomposition-group.md) equals its [inertia group](../../../../../../inertia-group.md).

Write $e=e(w/v_p)$. [Characteristic zero](../../../../../../characteristic-zero.md) makes all local ramification tame. One can choose a [uniformizer](../../../../../../uniformizer.md) $\pi$ in the completion for which

$$
u=\pi^e,\qquad E_w=F((\pi)),\qquad F(t)_{v_p}=F((u)).
$$

Indeed, initially $u$ is $\pi^e$ times a unit; that unit has an $e$th root in $F[[\pi]]$, by its algebraically closed residue [field](../../../../../../field.md) and the invertibility of $e$. Absorb it into $\pi$. The local automorphisms are then $\pi\mapsto\zeta\pi$, $\zeta\in\mu_e(F)$, and form a cyclic group of order $e$. Define $e_p=e$.

To specify an element rather than a subgroup, **fix a compatible choice of primitive [roots of unity](../../../../../../root-of-unity.md) $\zeta_e\in F$**. Define $\tau_w$ by its [uniformizer](../../../../../../uniformizer.md) character

$$
\overline{\tau_w(\pi)/\pi}=\zeta_e,
$$

and let $C_p$ be its [conjugacy class](../../../../../../conjugacy-class.md) in $G$. Over $\mathbb C$, take $\zeta_e=e^{2\pi i/e}$, corresponding to positive local continuation around $p$. At an unramified point, $e_p=1$ and $C_p=\{1\}$.

Changing the [uniformizer](../../../../../../uniformizer.md) does not affect this character. If $\pi'=a\pi$ with $a$ a unit, inertia fixes its residue, so

$$
\overline{\tau(\pi')/\pi'}
=\overline{\tau(a)/a}\,\overline{\tau(\pi)/\pi}
=\overline{\tau(\pi)/\pi}.
$$

The character is injective: a nonidentity finite-order automorphism with derivative one would have $\tau(\pi)=\pi+b\pi^r+\cdots$ for $r\geq2$, and its $N$th iterate would have coefficient $Nb$ at that first nonzero displacement. [Characteristic zero](../../../../../../characteristic-zero.md) contradicts finite order. Thus the chosen primitive character identifies a unique generator.

For another place $w'=\sigma w$, conjugation gives $D_{w'}=\sigma D_w\sigma^{-1}$, preserves its order, and carries $\tau_w$ to $\tau_{w'}$, since $\sigma$ fixes the constants and hence $\zeta_e$. This proves that $e_p$ and the [branch-cycle conjugacy class](../../../../../../branch-cycle-conjugacy-class.md) are independent of the place and [uniformizer](../../../../../../uniformizer.md). Without the stated roots-of-unity convention, only the cyclic inertia-subgroup [conjugacy class](../../../../../../conjugacy-class.md) is intrinsic: replacing $\zeta_e$ by another primitive root replaces the generator by a coprime power, which need not lie in the same [conjugacy class](../../../../../../conjugacy-class.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
