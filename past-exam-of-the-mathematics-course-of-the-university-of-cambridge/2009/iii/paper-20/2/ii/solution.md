<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A generator selects one point from each alpha circle and each beta circle. Here the points $1,3$ lie on $\alpha_1\cap\beta_2$, $2$ on $\alpha_1\cap\beta_1$, $a,c$ on $\alpha_2\cap\beta_1$, and $b$ on $\alpha_2\cap\beta_2$. Hence, with $R=\mathbb Z[U]$, the [Heegaard Floer chain complex](../../../../../../heegaard-floer-chain-complex.md) has free basis

$$
\boxed{(1,a),\ (1,c),\ (3,a),\ (3,c),\ (2,b).}
$$

A pair such as $(2,a)$ is invalid because it uses beta-one twice.

Orient the attaching circles so that their algebraic-intersection matrix is $\left(\begin{smallmatrix}1&-2\\-2&1\end{smallmatrix}\right)$. The presentation of $H_1(Y)$ is then $m_1-2m_2=0$, $m_2-2m_1=0$, giving $H_1(Y)=\mathbb Z/3$ with $m_2=-m_1$. The upper rectangular domain connects $(2,b)$ to $(3,c)$; the lower one connects $(2,b)$ to $(1,a)$. Thus these three generators have zero joining-cycle obstruction. Changing just the point on the second alpha circle from $a$ to $c$, or just the point on the first from $1$ to $3$, gives the two opposite nonzero meridian classes. This distinguishes the other two generators. The equivalence classes of [Whitney disk classes](../../../../../../whitney-disk-class.md) are therefore

$$
\boxed{\{(1,a),(2,b),(3,c)\},\qquad\{(1,c)\},\qquad\{(3,a)\}.}
$$

The dot in the central unshaded region represents the basepoint. Each displayed rectangle has $n_z=0$, Euler measure zero and four corner averages $1/4$, hence [Maslov index](../../../../../../maslov-index.md) one. The [relative grading in Heegaard Floer homology](../../../../../../relative-grading-in-heegaard-floer-homology.md) satisfies

$$
\operatorname{gr}(2,b)-\operatorname{gr}(1,a)=\operatorname{gr}(2,b)-\operatorname{gr}(3,c)=1.
$$

Thus a convenient normalization is **degree zero for $(1,a),(3,c)$ and degree one for $(2,b)$**; either singleton can independently be put in degree zero. As before, multiplication by $U^m$ subtracts $2m$ from every degree.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
