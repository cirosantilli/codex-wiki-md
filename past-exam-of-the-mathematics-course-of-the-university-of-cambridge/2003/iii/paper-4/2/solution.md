<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The isomorphic pair is $A_8\cong PSL_4(2)$; $PSL_3(4)$ is different.** All three have order $20160$, so order alone does not settle the question; explicitly $|PSL_3(4)|=(64-1)(64-4)(64-16)/(3\cdot3)=20160$. We give a concrete realization and an element-order distinction.

On $W=\bigwedge^2\mathbb F_2^4$, the [Pfaffian](../../../../../pfaffian.md) is

$$
Q(x)=x_{12}x_{34}+x_{13}x_{24}+x_{14}x_{23}.
$$

It is a nonsingular plus-type [quadratic form](../../../../../quadratic-form.md): the three displayed pairs give a hyperbolic decomposition. Change of [basis](../../../../../basis.md) multiplies the [Pfaffian](../../../../../pfaffian.md) by the [determinant](../../../../../determinant.md), which is always one in $GL_4(2)$. Hence the [exterior-square realization of PSL4 over F2](../../../../../exterior-square-realization-of-psl4-over-f2.md) embeds $GL_4(2)$ into $O_6^+(2)$. The [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is trivial: an element acting trivially on the [exterior square](../../../../../exterior-square.md) fixes every decomposable two-space, then every one-space as an intersection of two-spaces, and hence is a scalar; over $\mathbb F_2$ this scalar is one.

For a second model let $E$ be the even-weight [vector subspace](../../../../../vector-subspace.md) of $\mathbb F_2^8$ and quotient by the all-one vector. The dot product descends to a [nondegenerate](../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../alternating-bilinear-form.md) on the six-dimensional quotient, and

$$
q(\bar x)=\operatorname{wt}(x)/2\pmod2
$$

is well defined, since complementing an even subset changes half its weight from $w/2$ to $4-w/2$. It has $(1+70+1)/2=36$ zero vectors, so is plus type. Coordinate [permutations](../../../../../permutation.md) give a [faithful](../../../../../faithful-group-action.md) $S_8$ action: fixing the quotient fixes each weight-two subset, because its complement has weight six, and fixing all two-subsets forces the identity [permutation](../../../../../permutation.md).

From the independently derived symplectic order and quadratic orbit count below,

$$
|O_6^+(2)|=\frac{|Sp_6(2)|}{36}=40320,
\qquad |GL_4(2)|=(16-1)(16-2)(16-4)(16-8)=20160.
$$

Thus $O_6^+(2)\cong S_8$ and the image of $GL_4(2)=SL_4(2)=PSL_4(2)$ is its index-two [subgroup](../../../../../subgroup.md) $A_8$. The index-two [subgroup](../../../../../subgroup.md) is unique: a nontrivial [group homomorphism](../../../../../group-homomorphism.md) $S_8\to C_2$ sends every [transposition](../../../../../transposition-permutation.md) to the same nonidentity element and is the sign map.

To separate $PSL_3(4)$, observe that $A_8$ contains $(12345)(678)$ of order 15. An odd-order projective element of $PSL_3(4)$ lifts to a [semisimple linear operator](../../../../../semisimple-linear-operator.md), since its order upstairs divides three times an odd order in [characteristic](../../../../../characteristic-of-a-field.md) two. The possible [eigenspace](../../../../../eigenspace.md) degree patterns are $1+1+1$, $2+1$ and $3$. In the split case all [eigenvalues](../../../../../eigenvalue.md) have order dividing three, so the projective element has no order 15. In the $2+1$ case the [eigenvalues](../../../../../eigenvalue.md) are $\lambda,\lambda^4,\lambda^{-5}$ with $\lambda\in\mathbb F_{16}^\times$; its fifth power is scalar because $\lambda^{15}=1$, so its projective order divides five. In the irreducible case the determinant-one torus has order $4^2+4+1=21$ and quotienting its scalar [subgroup](../../../../../subgroup.md) of order three gives projective order dividing seven. **There is therefore no element of order 15 in $PSL_3(4)$.**

Several small-parameter coincidences connect the finite [classical groups](../../../../../classical-group.md) to [permutation groups](../../../../../permutation-group.md). The projective-line action immediately gives $PSL_2(2)\cong S_3$, $PSL_2(3)\cong A_4$, $PGL_2(3)\cong S_4$ and $PSL_2(4)\cong A_5$ by [faithful](../../../../../faithful-group-action.md) actions of degrees three, four and five and their orders. Also $PSL_2(5)\cong A_5$: its involutions have Klein-four [centralizers](../../../../../centralizer.md), giving five [Sylow subgroups](../../../../../sylow-subgroup.md); their [conjugation action](../../../../../conjugation-action.md) is [faithful](../../../../../faithful-group-action.md) and embeds its order-60 [simple group](../../../../../simple-group.md) into $S_5$. Simplicity here can be checked from class sizes $1,15,20,12,12$: no proper nontrivial normal class union has order dividing 60. The same five-subgroup action extends to $PGL_2(5)$, with trivial [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) and order 120, giving $S_5$. Indeed its kernel intersects $PSL_2(5)$ trivially, so centralizes that normal [subgroup](../../../../../subgroup.md). Commuting projectively with both upper and lower elementary unipotents forces a representing matrix to be scalar, so this kernel is trivial.

The less immediate coincidence $PSL_2(9)\cong A_6$ can be exhibited on the ten unordered triple partitions used in Question 4. Let $a=(123)$, $b=(456)$, $w=(12)(36)$, assign $\infty$ to $123\mid456$ and $0$ to $126\mid345$, and label the other partitions by applying $a^xb^y$ to the zero partition, with $t=x+iy\in\mathbb F_9$ and $i^2=-1$. Inspection of these nine partitions gives

$$
a:t\mapsto t+1,\qquad b:t\mapsto t+i,\qquad w:t\mapsto-1/t.
$$

Translations and inversion generate $PSL_2(9)$: conjugating the upper unitriangular matrices by inversion gives the lower ones, and elementary elimination generates $SL_2(9)$. Their projective action has order $9(9^2-1)/2=360$. These partition [permutations](../../../../../permutation.md) come from even [permutations](../../../../../permutation.md) of six letters, whose partition action is [faithful](../../../../../faithful-group-action.md) as proved below; hence they fill $A_6$.

Finally, on the even-weight module of $\mathbb F_2^6$ modulo its all-one vector, coordinate [permutations](../../../../../permutation.md) preserve a [nondegenerate](../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../alternating-bilinear-form.md) in [dimension](../../../../../dimension-vector-space.md) four and act faithfully, again by the weight-two-subset argument. Both $S_6$ and $Sp_4(2)$ have order 720, proving $Sp_4(2)\cong S_6$, with [commutator subgroup](../../../../../commutator-subgroup.md) $A_6$. These examples illustrate both the need to quotient [group centers](../../../../../center-of-a-group.md) and the low-rank exceptions to general simplicity. They do not make equal orders sufficient for [group isomorphism](../../../../../group-isomorphism.md), as the two order-20160 examples already demonstrate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
