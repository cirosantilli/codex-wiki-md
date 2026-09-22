<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove Booleanity directly from the dense-cover description. Let $B$ be a subsheaf of a sheaf $F$. Its pseudocomplement $N$ consists of sections $x\in F(c)$ such that no restriction along any arrow into $c$ belongs to $B$. This is a subpresheaf. It is also a sheaf: if a section of $F$ restricts into $N$ on a dense covering [sieve on a category](../../../../../../sieve-category-theory.md), any hypothetical restriction into $B$ has a further restriction in that cover; it would then belong to both $B$ and $N$, impossible. Thus the unique amalgamation in $F$ of an $N$-matching family lies in $N$.

For any $x\in F(c)$, the [sieve on a category](../../../../../../sieve-category-theory.md) of arrows on which its restriction lies in $B$ or $N$ is dense. Given an arrow $u:d\to c$, either some further restriction belongs to $B$, supplying the required member of that [sieve on a category](../../../../../../sieve-category-theory.md), or none does, in which case the restriction along $u$ itself belongs to $N$. Therefore $B\cup N$ is locally all of $F$, so their join in the [sheaf topos](../../../../../../grothendieck-topos.md) is $F$. Their intersection is empty. Every subsheaf consequently has a complement, proving **the topos is Boolean**.

For two-valuedness, let $U\hookrightarrow1$ be a nonempty subterminal sheaf. At some stage $m$, its value is the singleton. For every $k\ge m$ there is an arrow $k\to m$, so restriction makes $U(k)$ the singleton as well. At any stage $n$, the [sieve on a category](../../../../../../sieve-category-theory.md) of arrows into $n$ whose domains are at least $m$ is dense: after an arrow with domain $l$, choose a further domain $k\ge\max(l,m)$ and use the existence of arrows downwards. On this covering [sieve on a category](../../../../../../sieve-category-theory.md) the unique terminal section has a matching family in $U$, so the sheaf condition gives $U(n)=1$. Hence $U=1$. Since the empty [sieve on a category](../../../../../../sieve-category-theory.md) never covers, the empty presheaf is an initial sheaf distinct from $1$. Thus

$$
\boxed{\operatorname{Sub}(1)=\{0,1\},}
$$

and **the topos is two-valued**, in the distinct global sense of a [two-valued topos](../../../../../../two-valued-topos.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
