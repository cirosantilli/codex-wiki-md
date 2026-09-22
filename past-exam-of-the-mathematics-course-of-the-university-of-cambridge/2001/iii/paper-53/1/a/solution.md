<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The image of the full interval under the [tent map](../../../../../../tent-map.md) is $T_s([-1,1])=[1-s,1]$. Since $s>1$, this image contains the [critical point](../../../../../../critical-point.md) zero and the right endpoint one; its next image is again $[1-s,1]$. Moreover, any interval $B$ with $T_s(B)=B$ lies inside the image of $[-1,1]$. Thus the [core interval of an expanding tent map](../../../../../../core-interval-of-an-expanding-tent-map.md) is

$$
\boxed{A=[1-s,1]=[T_s^2(0),T_s(0)].}
$$

Every point outside $A$ enters $A$ after one iterate and then stays there. For $s=2$ there are no points of the domain outside $A$.

To prove [interval exactness of a tent-map core](../../../../../../interval-exactness-of-a-tent-map-core.md), first take a nondegenerate [closed interval](../../../../../../closed-real-interval.md) $L\subseteq A$ and put $L_n=T_s^n(L)$. Each $L_n$ is an interval. If $L_n$ does not straddle zero, the corresponding branch is affine with slope of magnitude $s$, so $|L_{n+1}|=s|L_n|$. If it straddles zero, its image has right endpoint one and

$$
|L_{n+1}|=s\max\{|\inf L_n|,|\sup L_n|\}\geq\frac{s}{2}|L_n|.
$$

If both $L_n$ and $L_{n+1}$ contain zero, then $L_{n+1}$ contains $[0,1]$, whence $L_{n+2}=A$. Otherwise at most one of these two steps folds across the [critical point](../../../../../../critical-point.md). Consequently, unless the full core has already been reached,

$$
|L_{n+2}|\geq\frac{s^2}{2}|L_n|.
$$

Since $s^2/2>1$, indefinite failure to reach $A$ would give intervals of unbounded length inside an interval of length $s$. This is impossible, proving $\boxed{T_s^k(L)=A\text{ for some }k}$. For an interval with open endpoints, apply the argument to any nondegenerate closed subinterval inside it; its image already covers $A$, while the image of the original interval cannot leave $A$.

Now let $U$ be any nonempty relatively open subset of $A$ and choose a closed nondegenerate $J=[u,v]\subset U$. Some $F=T_s^k$ maps $J$ onto $A$, so there are points $p,q\in J$ with $F(p)=1-s$ and $F(q)=1$. Therefore $F(p)-p\leq0$ and $F(q)-q\geq0$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) yields $z\in J$ with $F(z)=z$. This is a [periodic point](../../../../../../periodic-point.md) of $T_s$, of period dividing $k$. Every such $U$ contains one, so **the [periodic points](../../../../../../periodic-point.md) are dense in the whole core $A$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
