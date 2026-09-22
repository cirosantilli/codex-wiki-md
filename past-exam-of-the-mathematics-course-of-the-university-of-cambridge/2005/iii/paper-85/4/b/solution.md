<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The descending powers $J\supseteq J^2\supseteq\cdots$ stabilize because they are [right ideals](../../../../../../right-ideal.md). Choose $m\ge1$ with $J^m=J^{m+1}$ and put $I=J^m$. Then $I=J^{2m}=I^2$.

Suppose $I\ne0$. Among the [right ideals](../../../../../../right-ideal.md) $K$ such that $KI\ne0$, choose a minimal one; the set is nonempty since $RI=I\ne0$. The [right ideal](../../../../../../right-ideal.md) $KI$ lies in $K$, and $(KI)I=KI^2=KI\ne0$, so minimality forces $KI=K$. Choose $k\in K$ with $kI\ne0$. Then $(kR)I=kI\ne0$, and $kR\subseteq K$, so the same minimality gives $K=kR$.

Since $K=KI$ and $I\subseteq J$, its generator satisfies $k=\sum_\nu kr_\nu i_\nu=kj$ for an element $j=\sum_\nu r_\nu i_\nu\in J$. Thus $k(1-j)=0$. The [unit criterion for the Jacobson radical](../../../../../../unit-criterion-for-the-jacobson-radical.md) makes $1-j$ invertible, implying $k=0$, contrary to $kI\ne0$. Therefore $I=0$, and

$$
\boxed{J(R)^m=0.}
$$

The [minimal-right-ideal proof of radical nilpotence](../../../../../../minimal-right-ideal-proof-of-radical-nilpotence.md) is important here: one cannot apply the finite-generator form of [Nakayama lemma](../../../../../../nakayama-lemma.md) directly to $J^m$ before proving it finitely generated. We made a suitable auxiliary [right ideal](../../../../../../right-ideal.md) cyclic before using the unit argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
