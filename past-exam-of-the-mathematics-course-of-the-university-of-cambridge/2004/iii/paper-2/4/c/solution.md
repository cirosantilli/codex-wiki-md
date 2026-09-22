<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S=SL_n(F)$ and let $Z$ be its scalar center. Its action on the lines of $F^n$ has [kernel](../../../../../../kernel-of-a-linear-map.md) exactly $Z$: a [linear map](../../../../../../linear-map.md) fixing every line is diagonal in a basis, and fixing the lines spanned by $e_i+e_j$ makes all its diagonal entries equal. The action is two-transitive. Indeed an ordered pair of distinct lines can be represented by two independent [vectors](../../../../../../vector.md) and extended to a basis. A [linear map](../../../../../../linear-map.md) between two such bases can be adjusted to [determinant](../../../../../../determinant.md) one by scaling one target basis [vector](../../../../../../vector.md); this preserves both target lines. Therefore $S/Z$ has a faithful [primitive group action](../../../../../../primitive-group-action.md).

Fix $L=Fv$. The maps

$$
A_L=\{I+vf:f\in(F^n)^*,\ f(v)=0\}
$$

form an abelian [subgroup](../../../../../../subgroup.md): all products of the rank-one terms vanish. It is normal in the line stabilizer, since [conjugation](../../../../../../conjugation.md) replaces $v$ by a [scalar multiple](../../../../../../scalar-multiple.md) and transports $f$. Its conjugates contain every [transvection](../../../../../../transvection.md), and hence generate $S$ by 4(b). The same statements hold for its [image](../../../../../../image-of-a-function.md) in $S/Z$.

It remains to prove perfectness rather than assume it. Use the [group commutator](../../../../../../group-commutator.md) convention $[x,y]=xyx^{-1}y^{-1}$. If $n\ge3$, distinct $i,j,k$ give

$$
[x_{ik}(a),x_{kj}(b)]=x_{ij}(ab).
$$

Every elementary generator is consequently in $S'$. If $n=2$ and $|F|>3$, choose $a\in F^*$ with $a^2\ne1$. There are at most two roots of $a^2=1$, so such a choice exists. For $h=\operatorname{diag}(a,a^{-1})$,

$$
[h,x_{12}(b)]=x_{12}((a^2-1)b).
$$

Varying $b$ gives every upper [transvection](../../../../../../transvection.md); conjugating by $w(1)$ gives every lower one. Again $S'=S$, and its projective quotient is a [perfect group](../../../../../../perfect-group.md).

Apply 4(a) to this faithful primitive projective action. Every nontrivial [normal subgroup](../../../../../../normal-subgroup.md) contains the [commutator subgroup](../../../../../../commutator-subgroup.md), which is the whole quotient. Thus

$$
\boxed{PSL_n(F)\text{ is simple if }n\ge3\text{ or if }n=2,\ |F|>3.}
$$

The restriction is real: $PSL_2(2)\cong S_3$ and $PSL_2(3)\cong A_4$ are not simple.

## ↑ Ancestors (11)

1. [C](../c.md)
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
