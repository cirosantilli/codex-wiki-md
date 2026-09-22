<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For any integer $n\geq1$, let $R=R_{2\pi/n}$ in the [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) from [i](../i.md). Since $R_\theta R_\phi=R_{\theta+\phi}$ and $R_\theta=I$ exactly when $\theta\in2\pi\mathbb Z$, this [rotation matrix](../../../../../../../rotation-matrix.md) has order exactly $n$. Therefore

$$
\boxed{\langle R_{2\pi/n}\rangle\cong C_n}
$$

is a [subgroup](../../../../../../../subgroup.md) of $G$ of order $n$, including the trivial case $n=1$.

For infinitely many non-Abelian examples, let $n\geq3$, retain $R=R_{2\pi/n}$, and take the half-turn

$$
J=\operatorname{diag}(-1,1,-1)\in G.
$$

Direct multiplication gives $J^2=I$ and $JRJ=R^{-1}$. Every word in $R,J$ therefore reduces to $R^k$ or $R^kJ$, $0\leq k<n$. The $R^k$ are distinct, as are the $R^kJ$, and no element from the first family equals one from the second: they send $N$ to $N$ and $-N$, respectively. Hence $\langle R,J\rangle$ has exactly $2n$ elements and is a [dihedral group](../../../../../../../dihedral-group.md).

It is non-Abelian because $R\ne R^{-1}$ for $n\geq3$, so $JR\ne RJ$. Different values of $n$ give different [group orders](../../../../../../../order-of-a-finite-group.md), and therefore different [subgroups](../../../../../../../subgroup.md). Thus **$G$ has infinitely many non-Abelian subgroups**, already among its finite [subgroups](../../../../../../../subgroup.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
