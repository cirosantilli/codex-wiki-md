<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

In [Glendinning chaos](../../../../../glendinning-chaos.md), a continuous [interval map](../../../../../interval-map.md) is chaotic when some positive iterate has a [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md). In the interval version, one may take an open interval $J$ containing two disjoint open intervals $K_0,K_1$ with $F^m(K_0)=F^m(K_1)=J$.

Let a three-cycle be ordered $a<b<c$. There are only two possible cyclic orderings; reflection of the coordinate interchanges them, so assume $F(a)=b$, $F(b)=c$, $F(c)=a$. Then

$$
F^2(a)=c,\qquad F^2(b)=a.
$$

Also $F(b)=c$ and $F(c)=a$, so the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives $d\in(b,c)$ with $F(d)=b$, whence $F^2(d)=c$. Both $[a,b]$ and $[b,d]$ therefore map across $[a,c]$ under $F^2$.

To obtain exact open-interval images, use the following elementary first-passage observation. A continuous function on $[r,s]$ with endpoint values $a,c$ has a subinterval on which its endpoint values are $a,c$ and all interior values lie strictly between them: take the first hit of the second level, then the last hit of the first level before it. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) makes its interior image exactly $(a,c)$. Apply this to the two intervals, reversing endpoint order on the first. Their selected interiors $K_0\subset(a,b)$ and $K_1\subset(b,d)$ are disjoint and lie in $J=(a,c)$, with

$$
\boxed{F^2(K_0)=F^2(K_1)=J.}
$$

This proves the [three-cycle forces a two-iterate interval horseshoe](../../../../../three-cycle-forces-a-two-iterate-interval-horseshoe.md) result and establishes the required horseshoe for $F^2$.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
