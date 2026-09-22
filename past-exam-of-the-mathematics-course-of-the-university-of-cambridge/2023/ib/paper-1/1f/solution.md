<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Choose [bases](../../../../../basis.md) of $V$ and $W$, of dimensions $v$ and $w$. A [linear map](../../../../../linear-map.md) is uniquely determined by the arbitrary images of the $v$ [basis](../../../../../basis.md) [vectors](../../../../../vector.md), each with $w$ coordinates, so

$$
\dim L(V,W)=vw.
$$

Put $a=\dim A$ and $b=\dim B$, and extend [bases](../../../../../basis.md) of $A,B$ to [bases](../../../../../basis.md) of $V,W$. The condition $\phi(A)\subseteq B$ forces the $(w-b)a$ [matrix](../../../../../matrix.md) entries from $A$ to a complement of $B$ to vanish and imposes no other restriction. Hence

$$
\dim X=vw-a(w-b).
$$

For the last part let $r=\dim(S\cap T)=s+t-v$. Choose

$$
V=(S\cap T)\oplus S_0\oplus T_0.
$$

A map in $Y$ sends $S\cap T$ into itself, $S_0$ into $S$, and $T_0$ into $T$, with these choices independent. Therefore

$$
\boxed{\dim Y=r^2+s(s-r)+t(t-r),
\qquad r=s+t-v.}
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
