<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V=F^n$ and let $G=PSL(n,F)$ act on its one-dimensional subspaces. First identify the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) in $SL(n,F)$. A [matrix](../../../../../../matrix.md) fixing every coordinate line is diagonal, and fixing every line $\langle e_i+e_j\rangle$ forces all diagonal entries equal. Thus the projective [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is $\{\lambda I:\lambda^n=1\}$. These scalars are central. Conversely a central [matrix](../../../../../../matrix.md) commutes with all $E_{ij}(1)$: comparing entries in $Me_{ij}=e_{ij}M$ shows all off-diagonal entries of $M$ vanish and all diagonal entries agree. Therefore the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is exactly $Z(SL(n,F))$. This proves [scalar kernel of the projective linear action](../../../../../../scalar-kernel-of-the-projective-linear-action.md) and faithfulness of the induced $G$-action.

The action is doubly transitive. Given two ordered pairs of distinct lines, choose two independent representatives of each pair and extend them to [bases](../../../../../../basis.md). A [linear map](../../../../../../linear-map.md) taking the first [basis](../../../../../../basis.md) to the second sends the desired lines correctly. If its [determinant](../../../../../../determinant.md) is $d\ne1$, postcompose with a diagonal map in the target [basis](../../../../../../basis.md) that scales its first [basis](../../../../../../basis.md) [vector](../../../../../../vector.md) by $d^{-1}$ and fixes all the others. It preserves the two target lines and corrects the [determinant](../../../../../../determinant.md). Thus an element of $SL(n,F)$ sends either ordered pair to the other. Double transitivity implies primitivity: a block containing two distinct points must contain every point by the transitive point-stabilizer action.

For $\alpha=\langle e_1\rangle$, consider

$$
U=\{I+e_1\varphi:\varphi\in V^*,\ \varphi(e_1)=0\}.
$$

Products add the functionals, so $U$ is abelian. If $g$ fixes $\alpha$, write $ge_1=ae_1$. Then $g(I+e_1\varphi)g^{-1}=I+e_1(a\varphi g^{-1})$, and the new functional still vanishes on $e_1$. Thus the image $A$ of $U$ in $G$ is normal in the [point stabilizer](../../../../../../stabilizer-subgroup.md). Its conjugates contain all elementary [transvections](../../../../../../transvection.md): changing the center line $\langle e_1\rangle$ to $\langle e_i\rangle$ gives every map $I+e_i\psi$ with $\psi(e_i)=0$, including $E_{ij}(t)$. Part (b) then shows that those conjugates generate $G$.

It remains to prove perfectness, not assume it. Use $[x,y]=x^{-1}y^{-1}xy$. For $n\geq3$, distinct $i,j,k$ give

$$
[E_{ik}(t),E_{kj}(1)]=E_{ij}(t).
$$

Every generator is therefore a [group commutator](../../../../../../group-commutator.md), so $SL(n,F)'=SL(n,F)$. For $n=2$ and $|F|>3$, choose $a\in F^\times$ with $a^2\ne1$, possible because a quadratic polynomial has at most two roots. With $D=\operatorname{diag}(a,a^{-1})$,

$$
[D,E_{12}(t)]=E_{12}((1-a^{-2})t),\qquad
[D,E_{21}(t)]=E_{21}((1-a^2)t).
$$

Both coefficients are nonzero, so every upper and lower elementary [transvection](../../../../../../transvection.md) is again a [group commutator](../../../../../../group-commutator.md). Part (b) proves perfectness in this case as well. Quotients of perfect [groups](../../../../../../group-split.md) are perfect, hence $G'=G$ in exactly the stated range.

Apply part (a) to the faithful primitive $G$-action and its abelian normal point-stabilizer [subgroup](../../../../../../subgroup.md) $A$. Every nontrivial [normal subgroup](../../../../../../normal-subgroup.md) contains $G'=G$, so it is the whole [group](../../../../../../group-split.md). A [transvection](../../../../../../transvection.md) is not scalar, showing $G\ne1$. We have proved

$$
\boxed{PSL(n,F)\text{ is simple for }n\geq3,\text{ or }n=2\text{ with }|F|>3.}
$$

The proof works for infinite [fields](../../../../../../field.md) too and uses no finite-order count. The excluded two-dimensional [fields](../../../../../../field.md) give the familiar soluble exceptions $PSL(2,2)\cong S_3$ and $PSL(2,3)\cong A_4$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
