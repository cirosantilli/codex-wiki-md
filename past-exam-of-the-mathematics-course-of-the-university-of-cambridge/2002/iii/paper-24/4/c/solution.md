<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), and write $N_p=\#\widetilde E(\mathbb F_p)$. The [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md) and the [formal group law](../../../../../../formal-group-law.md) determine the torsion as follows. If $p\nmid n$, multiplication by $n$ is an automorphism of $E_1$, because its multiplication series has an integral compositional inverse with unit linear coefficient. Therefore reduction gives an isomorphism

$$
E(\mathbb Q_p)[n]\cong\widetilde E(\mathbb F_p)[n].
$$

To construct the inverse, lift a reduced point to $P$, solve $[n]Q=[n]P$ uniquely in $E_1$, and use $P-Q$. This proves the [prime-to-p torsion lifts uniquely at good reduction](../../../../../../prime-to-p-torsion-lifts-uniquely-at-good-reduction.md), including uniqueness, rather than merely comparing orders.

For residue-characteristic torsion, use a [deep logarithm subgroup of a formal group](../../../../../../deep-logarithm-subgroup-of-a-formal-group.md). Take $m=1$ for odd $p$, or $m=2$ at two. The [formal logarithm](../../../../../../formal-logarithm.md) identifies $E_m$ with $p^m\mathbb Z_p$, so $E_m$ has no torsion. The finite [quotient group](../../../../../../quotient-group.md)

$$
G=E(\mathbb Q_p)/E_m,\qquad |G|=N_p p^{m-1},
$$

therefore receives the [torsion subgroup](../../../../../../torsion-subgroup.md) injectively. There is a complete test for which cosets actually contain torsion. For a coset $g$ of order $n$, choose a lift $P$. Then $[n]P\in E_m$. Its coset has a torsion representative exactly when

$$
\boxed{L([n]P)\in n p^m\mathbb Z_p.}
$$

When this condition holds, let $Q\in E_m$ be the unique point with $L(Q)=L([n]P)/n$. Then $T=P-Q$ is killed by $n$ and represents $g$. Conversely, any torsion representative has order precisely $n$, since an element killed in the quotient would belong to the torsion-free group $E_m$. It must therefore arise from this construction. Changing $P$ by $R\in E_m$ changes $L([n]P)$ by $nL(R)$, so the test is independent of the chosen lift. This proves the [torsion test using a deep formal logarithm subgroup](../../../../../../torsion-test-using-a-deep-formal-logarithm-subgroup.md) and gives the full torsion by a finite list of cosets and a logarithmic divisibility test.

For odd $p$, one has $E_m=E_1$, so all [torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) inject into $\widetilde E(\mathbb F_p)$. Nevertheless a reduced $p$-primary point need not lift to a torsion point: if its order is $p^r$, the test is $L([p^r]P)\in p^{r+1}\mathbb Z_p$. For $p=2$, the subgroup $E_2$ is torsion-free but $E_1/E_2$ has order two. Thus $E_1$ can have a two-torsion point, and one must use $G=E/E_2$ of order $2N_2$ rather than assert that all torsion injects under reduction. The [prime-two torsion bound for good reduction](../../../../../../prime-two-torsion-bound-for-good-reduction.md) follows: the reduction kernel contributes at most a subgroup of order two. These distinctions are essential to a correct determination of local [torsion subgroups](../../../../../../torsion-subgroup.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
