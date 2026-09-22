<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $R=\mathbb Z[U]$, with $\deg U=-2$. In [genus](../../../../../../genus-of-a-surface.md) one, an intersection point is itself a generator of the [Heegaard Floer chain complex](../../../../../../heegaard-floer-chain-complex.md). Thus the free $R$ basis is

$$
\boxed{1,2,3,4,5,6,7.}
$$

There are infinitely many integral generators $U^m j$, $m\ge0$, but these seven points are the module generators.

The obstruction to a [Whitney disk class](../../../../../../whitney-disk-class.md) is the alpha-and-beta joining cycle in $H_1(Y)$. Identify the opposite sides of the square and straighten the two small fingers of the alpha curve. Its algebraic intersection with beta is three; the remaining intersections, one in each residue class, are represented by $1,4,5$. The four small bigons connect $1$ to $2$ to $3$, and $5$ to $6$ to $7$. A joining cycle between consecutive remaining strands is a meridian, which generates $H_1(Y)=\mathbb Z/3$. Consequently the equivalence classes are exactly

$$
\boxed{\{1,2,3\},\qquad\{4\},\qquad\{5,6,7\}.}
$$

Equivalently, these are the three [Spin-c structures](../../../../../../spin-c-structure.md) represented in the [Heegaard diagram](../../../../../../heegaard-diagram.md).

Use the domain convention $\partial_\alpha D=y-x$. The positive bigons run from $2$ to $1$, from $2$ to $3$, from $5$ to $6$, and from $7$ to $6$. Their [Maslov indices](../../../../../../maslov-index.md) are one: their Euler measure is $1/2$, and the two endpoint averages contribute $1/4$ each. Write their basepoint multiplicities as $a,b,c,d$, respectively. The [relative grading in Heegaard Floer homology](../../../../../../relative-grading-in-heegaard-floer-homology.md) is therefore

$$
\boxed{\begin{aligned}
\operatorname{gr}(2)-\operatorname{gr}(1)&=1-2a,&\operatorname{gr}(2)-\operatorname{gr}(3)&=1-2b,\\
\operatorname{gr}(5)-\operatorname{gr}(6)&=1-2c,&\operatorname{gr}(7)-\operatorname{gr}(6)&=1-2d.
\end{aligned}}
$$

The reproduced figure has no visible marked $z$. If $z$ is outside all four small bigons, as in the usual intended diagram, $a=b=c=d=0$. One may normalize the [relative Heegaard Floer gradings](../../../../../../relative-grading-in-heegaard-floer-homology.md) as

$$
\boxed{(\operatorname{gr}1,\operatorname{gr}2,\operatorname{gr}3)=(0,1,0),\quad\operatorname{gr}4=0,\quad(\operatorname{gr}5,\operatorname{gr}6,\operatorname{gr}7)=(1,0,1).}
$$

Each class has its own arbitrary additive constant, and $\operatorname{gr}(U^m j)=\operatorname{gr}(j)-2m$. If the basepoint is put inside one of these disjoint bigons, exactly its multiplicity is one; the preceding boxed difference formulas give the answer without an unstated basepoint assumption.

## ↑ Ancestors (11)

1. [I](../i.md)
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
