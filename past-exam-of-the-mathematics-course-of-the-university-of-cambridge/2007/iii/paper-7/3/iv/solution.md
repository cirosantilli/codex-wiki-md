<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the [group commutator](../../../../../../group-commutator.md) convention $[x,y]=x^{-1}y^{-1}xy$. If $n\ge3$, choose distinct $i,j,k$. Multiplying elementary matrices, using $E_{ik}E_{kj}=E_{ij}$ and all reverse or repeated products here equal to zero, gives

$$
[x_{ik}(a),x_{kj}(1)]=x_{ij}(a).
$$

Every elementary generator is therefore in the [commutator subgroup](../../../../../../commutator-subgroup.md). Part iii shows these generators generate $\operatorname{SL}(V)$, proving it is a [perfect group](../../../../../../perfect-group.md).

It remains to handle $n=2$ and $q>3$. The polynomial $s^2-1$ has at most two roots, whereas $\mathbb F_q^\times$ has more than two elements, so choose $s\ne0$ with $s^2\ne1$. For $h=\operatorname{diag}(s,s^{-1})$, direct conjugation gives

$$
[h,x_{12}(t)]=x_{12}((1-s^{-2})t),\qquad [h,x_{21}(t)]=x_{21}((1-s^2)t).
$$

Both coefficients are nonzero. As $t$ varies, these [group commutators](../../../../../../group-commutator.md) give every upper and lower elementary [transvection](../../../../../../transvection.md), which generate $\operatorname{SL}_2(\mathbb F_q)$. Thus the [perfectness of the special linear group](../../../../../../perfectness-of-the-special-linear-group.md) is established in all requested cases:

$$
\boxed{\operatorname{SL}_n(\mathbb F_q)'=\operatorname{SL}_n(\mathbb F_q)\quad\text{if }n\ge2,\ (n,q)\notin\{(2,2),(2,3)\}.}
$$

The two pairs in the PDF are exclusions, not a literal logical disjunction. They really are exceptions: $\operatorname{SL}_2(\mathbb F_2)\cong S_3$ has a nontrivial sign quotient. Also $\operatorname{SL}_2(\mathbb F_3)$ maps onto $\operatorname{PSL}_2(\mathbb F_3)\cong A_4$, which has the nontrivial abelian quotient $A_4/V_4\cong C_3$. For the latter identification, the faithful projective action has degree four and image of order 12, hence the index-two subgroup $A_4$ of $S_4$. Neither exceptional group is perfect.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
