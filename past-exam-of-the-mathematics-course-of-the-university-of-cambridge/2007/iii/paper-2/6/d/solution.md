<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $n:k\to V^*\otimes V$ be the supplied [coevaluation morphism](../../../../../../coevaluation-morphism.md), $n(1)=x\otimes u+y\otimes v$, and let $e:V^*\otimes V\to k$ be the supplied [evaluation morphism](../../../../../../evaluation-morphism.md) with diagonal coefficients $A,B$. The [tangle](../../../../../../tangle.md) obtained by inserting the given crossing between the created strand and a through strand, then evaluating, is a removable curl. The first [Reidemeister move](../../../../../../reidemeister-move.md) gives the identity

$$
(e\otimes1_V)(1_{V^*}\otimes c)(n\otimes1_V)=1_V.
$$

We calculate this map on both [basis](../../../../../../basis.md) vectors. The crossing matrix gives

$$
\begin{aligned}
c(u\otimes u)&=q^{-1}u\otimes u,\\
c(u\otimes v)&=q^{-2}v\otimes u,\\
c(v\otimes u)&=q^{-2}u\otimes v+q^{-2}(q-q^{-1})v\otimes u,\\
c(v\otimes v)&=q^{-1}v\otimes v.
\end{aligned}
$$

For input $u$, applying $n$, then $c$, then $e$ gives

$$
\left[q^{-1}A+q^{-2}(q-q^{-1})B\right]u.
$$

For input $v$, the off-diagonal evaluation vanishes and the result is $q^{-1}Bv$. Therefore the removable-curl identity requires

$$
q^{-1}B=1,\qquad q^{-1}A+q^{-2}(q-q^{-1})B=1.
$$

Solve the first equation to obtain $B=q$; substitution in the second gives $A=q^{-1}$. Hence

$$
\boxed{A=q^{-1},\qquad B=q.}
$$

Finally the closed identity strand is represented by $e\circ n$. Its value is $e(x\otimes u+y\otimes v)=A+B$, so the [quantum dimension](../../../../../../quantum-dimension.md) is

$$
\boxed{\dim_q(V)=q^{-1}+q=[2].}
$$

It is a weighted categorical contraction, rather than the ordinary [vector space](../../../../../../vector-space-split.md) dimension $2$. Using a framed category without imposing the removable-curl identity would require additional twist data; the ordinary [tangle category](../../../../../../tangle-category.md) and the specified crossing normalization determine these coefficients.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
