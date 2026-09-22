<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $x\in J$ and put $u=1+yx$. If the [left ideal](../../../../../../left-ideal.md) $Au$ were proper, it would lie in a [maximal left ideal](../../../../../../maximal-left-ideal.md) $L$. But $yx\in J\subseteq L$, so $u\in L$ would imply $1\in L$. Thus $Au=A$, and $u$ has a left inverse $v$ with $vu=1$.

A left inverse alone is insufficient in a general operator algebra. Here $v=1-vyx$ differs from the identity by an element of $J$. The same argument supplies a left inverse $w$ of $v$. Then $w=w(vu)=(wv)u=u$, hence $uv=wv=1$. So $u$ is genuinely invertible.

Conversely, if $x\notin J$, part (i) gives a maximal left ideal $L$ with $x\notin L$. Maximality implies $L+Ax=A$, so $1=l+ax$ for some $l\in L,a\in A$. Therefore $1-ax=l\in L$ cannot be invertible, since a proper left ideal contains no invertible element. Taking $y=-a$ disproves the required universal invertibility. We have proved the [unit criterion for the Jacobson radical](../../../../../../unit-criterion-for-the-jacobson-radical.md) in the requested form:

$$
\boxed{x\in J\iff 1+yx\text{ is invertible for every }y\in A.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
