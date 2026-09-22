<h1 id="12f/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $p=t-\lambda r$ using part (a). At every node,

$$
f(y_j)-p(y_j)=\lambda(-1)^j,\qquad \|f-p\|_{L^\infty(Y)}=|\lambda|.
$$

If $\lambda=0$, the error vanishes. Otherwise any degree-at-most-$n$ [polynomial](../../../../../../../polynomial-split.md) $q$ with strictly smaller error would make $q-p$ have alternating nonzero signs at the increasingly ordered nodes (reversed globally if $\lambda<0$). It would then have at least $n+1$ distinct roots by the [intermediate value theorem](../../../../../../../intermediate-value-theorem.md), impossible. Hence

$$
\boxed{p=t-\lambda r\text{ minimizes }\|f-q\|_{L^\infty(Y)}\text{ over }\deg q\leq n.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [12F](../../../12f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2011](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
