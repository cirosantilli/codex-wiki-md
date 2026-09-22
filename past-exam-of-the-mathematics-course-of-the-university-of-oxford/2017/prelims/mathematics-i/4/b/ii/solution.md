<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [tripotent linear operator](../../../../../../../tripotent-linear-operator.md), the relation $T^3=T$ gives $T(T^2-I)=0$. Since $T^2\ne I$, there is $v$ with $(T^2-I)v\ne0$, and that nonzero [vector](../../../../../../../vector.md) belongs to $\ker T$. Hence $n_T\geq1$. Also $T\ne0$, because $T=0$ would imply $T^2=T$. The [rank-nullity theorem](../../../../../../../rank-nullity-theorem.md) in [dimension](../../../../../../../dimension-vector-space.md) three therefore gives

$$
\boxed{n_T\in\{1,2\}.}
$$

Now suppose $n_T=2$. Then $\operatorname{im}T$ is a line. On this line, $T^2$ is the [identity operator](../../../../../../../identity-operator.md): if $y=Tx$, then $T^2y=T^3x=Tx=y$. Consequently $T$ acts on this line by a [scalar](../../../../../../../scalar.md) $c$ satisfying $c^2=1$. If $c=1$, then $T^2x=Tx$ for every $x$, contrary to $T^2\ne T$. Thus $c=-1$.

Choose a nonzero $w\in\operatorname{im}T$, so $Tw=-w$. It does not belong to $\ker T$. A [basis](../../../../../../../basis.md) $k_1,k_2$ of $\ker T$, followed by $w$, is therefore a [basis](../../../../../../../basis.md) of $V$, in which

$$
\boxed{[T]_{(k_1,k_2,w)}=\begin{pmatrix}0&0&0\\0&0&0\\0&0&-1\end{pmatrix}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
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
