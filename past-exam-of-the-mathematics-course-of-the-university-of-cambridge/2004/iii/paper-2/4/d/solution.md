<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Replace $F^n$ by a [symplectic vector space](../../../../../../symplectic-vector-space.md) $(V,B)$ of dimension $2m$, and elementary row operations by [symplectic transvections](../../../../../../symplectic-transvection.md)

$$
T_{v,c}(x)=x+cB(x,v)v.
$$

The cross terms in $B(Tx,Ty)$ cancel, and $B(v,v)=0$, so these maps preserve $B$. Their inverses are $T_{v,-c}$.

They generate $Sp(V)$ by the following [symplectic basis](../../../../../../symplectic-basis.md) elimination. If $B(u,v)\ne0$, a single [transvection](../../../../../../transvection.md) with direction $v-u$ and parameter $1/B(u,v)$ sends $u$ to $v$. If $B(u,v)=0$ and $u\ne v$, choose $w$ with both $B(u,w)$ and $B(w,v)$ nonzero: the union of two proper [hyperplanes](../../../../../../hyperplane.md) does not exhaust a [vector space](../../../../../../vector-space-split.md), even over $\mathbb F_2$. Two [transvections](../../../../../../transvection.md) then suffice. Thus one can make a form-preserving [linear map](../../../../../../linear-map.md) fix the first basis [vector](../../../../../../vector.md) $e$. Next align its partner $f$, while keeping $e$ fixed. Two partners have difference in $e^\perp$, so the preceding single-transvection construction uses a direction in $e^\perp$ whenever their mutual pairing is nonzero. If it is zero, the intermediate partner $f+ae$, $a\ne0$, has nonzero pairing with both. All these [transvections](../../../../../../transvection.md) fix $e$. Once both $e,f$ are fixed, recurse on their [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) [symplectic orthogonal complement](../../../../../../symplectic-orthogonal-complement.md). This proves generation over every [field](../../../../../../field.md).

Use the action on the points of [projective space](../../../../../../projective-space-split.md), whose [kernel](../../../../../../kernel-of-a-linear-map.md) is the scalar center $Z=\{\lambda I:\lambda^2=1\}$. For $m=1$ this is the $SL_2$ case. For $m\ge2$ the action is primitive, although it is generally not two-transitive. The stabilizer of a line $L$ has two orbits on other lines: those orthogonal to $L$ and those not orthogonal to $L$. This follows by extending a [hyperbolic pair](../../../../../../hyperbolic-pair.md), or an independent isotropic pair, to a [symplectic basis](../../../../../../symplectic-basis.md). A block containing $L$ and a second line $M$ contains the entire corresponding orbit of the stabilizer of $L$. The stabilizer of $M$ then supplies a line of the other type: choose a [vector](../../../../../../vector.md) orthogonal to one of $L,M$ and not to the other. Nondegeneracy and independence guarantee such a [vector](../../../../../../vector.md), also in dimension four. Hence the block contains both orbits and is the whole set.

The [transvections](../../../../../../transvection.md) along $L$ form an abelian normal [subgroup](../../../../../../subgroup.md) of its stabilizer; their conjugates generate the [group](../../../../../../group-split.md). Thus the [Iwasawa simplicity lemma](../../../../../../iwasawa-simplicity-lemma.md) applies as soon as perfectness is established. For $|F|>3$, every [transvection](../../../../../../transvection.md) lies in an embedded $SL_2(F)$ acting on a hyperbolic plane, and 4(c) proves that embedded [group](../../../../../../group-split.md) perfect.

For the remaining fields, the [perfectness of finite symplectic groups](../../../../../../perfectness-of-finite-symplectic-groups.md) has a short direct proof. Over $\mathbb F_3$ with $m\ge2$, all parameter-one [transvections](../../../../../../transvection.md) have the same class $t$ in the [abelianization](../../../../../../abelianization.md), and $3t=0$. In an isotropic plane with basis $u,v$, the four directions $u,v,u+v,u-v$ give commuting [transvections](../../../../../../transvection.md) whose product is $1$: their rank-one terms add to zero, since

$$
uu^{\mathsf T}+vv^{\mathsf T}+(u+v)(u+v)^{\mathsf T}+(u-v)(u-v)^{\mathsf T}=0
$$

over $\mathbb F_3$. Thus $4t=0$, giving $t=0$. Parameter-two [transvections](../../../../../../transvection.md) are inverses, so all generators vanish in the [abelianization](../../../../../../abelianization.md). Over $\mathbb F_2$ with $m\ge3$, use the seven nonzero [vectors](../../../../../../vector.md) of an isotropic three-space. Their commuting [transvections](../../../../../../transvection.md) multiply to $1$, since each diagonal coordinate of $\sum_{0\ne v}vv^{\mathsf T}$ occurs four times and each off-diagonal coordinate twice. Their common abelianized class satisfies $2t=7t=0$, and again the [group](../../../../../../group-split.md) is perfect.

Consequently **the projective [symplectic group](../../../../../../symplectic-group.md) is simple**, with the necessary exceptions

$$
\boxed{PSp_{2m}(F)\text{ simple, except }(m,F)=(1,\mathbb F_2),(1,\mathbb F_3),(2,\mathbb F_2).}
$$

The first two are the linear exceptions; the last is $Sp_4(2)\cong S_6$, proved in 6(c). The word “projective” matters: the unquotiented [symplectic group](../../../../../../symplectic-group.md) may have the nontrivial scalar center $\{I,-I\}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
