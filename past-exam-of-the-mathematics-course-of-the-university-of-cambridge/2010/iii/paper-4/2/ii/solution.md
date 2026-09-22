<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the displayed formula as a right [group action](../../../../../../group-action.md): applying $(a,b)$ and then $(c,d)$ gives $(ac,bd)$. It is transitive since $(1,t)$ sends the identity to $t$. An element fixing every $t$ must have $a=b$ by evaluating at the identity, and then $a^{-1}ta=t$ for every $t$. Its kernel is therefore $\{(z,z):z\in Z(T)\}$, which is trivial by the [center of a group](../../../../../../center-of-a-group.md) hypothesis.

The identity [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) is $\Delta=\{(a,a):a\in T\}$. For every [subgroup](../../../../../../subgroup.md) $H$ containing $\Delta$, set

$$
N=\{b:(1,b)\in H\}.
$$

Conjugation by diagonal elements makes $N$ normal in $T$. Multiplying $(a,b)\in H$ by $(a,a)^{-1}$ shows $(1,a^{-1}b)\in H$, so

$$
H=\{(a,b):a^{-1}b\in N\}.
$$

Conversely each [normal subgroup](../../../../../../normal-subgroup.md) $N$ gives such an $H$. Thus the [subgroups](../../../../../../subgroup.md) strictly between $\Delta$ and $T\times T$ correspond exactly to proper nontrivial [normal subgroups](../../../../../../normal-subgroup.md) of $T$.

For a transitive action, blocks containing a chosen point correspond to [subgroups](../../../../../../subgroup.md) containing its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md): a block is the orbit of that point under its setwise [stabilizer subgroup](../../../../../../stabilizer-subgroup.md), and conversely the orbit under an intermediate [subgroup](../../../../../../subgroup.md) gives a block. Therefore the [diagonal action on a centerless group](../../../../../../diagonal-action-on-a-centerless-group.md) is primitive exactly when $T$ is simple. A nontrivial centerless [simple group](../../../../../../simple-group.md) cannot be abelian, because an abelian group's [center of a group](../../../../../../center-of-a-group.md) is the whole group. Hence

$$
\boxed{\text{The action is faithful and transitive, and primitive iff }T
\text{ is nonabelian simple}.}
$$

This uses the usual nontrivial degree convention. If one allows a one-point action to count as primitive, $T=1$ is the additional degenerate exception.

For the requested order example use $T=A_5$. Its simplicity follows from its conjugacy-class sizes $1,15,20,12,12$: a [normal subgroup](../../../../../../normal-subgroup.md) is a union of classes containing the identity, and no proper nontrivial such sum divides 60. Set $p=59$, a prime. The primitive diagonal action has

$$
\boxed{n=60=p+1,\qquad G=A_5\times A_5,\qquad |G|=3600,\quad59\nmid3600.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
