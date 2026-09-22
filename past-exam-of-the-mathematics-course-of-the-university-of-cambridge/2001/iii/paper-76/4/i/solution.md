<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

One quantitative form of the [Balog-Szemerédi-Gowers theorem](../../../../../../balog-szemeredi-gowers-theorem.md) is: if a nonempty finite set $A$ in an [abelian group](../../../../../../abelian-group.md) has $|A|=n$ and [additive energy](../../../../../../additive-energy.md) $E(A)\ge\eta n^3$, where $0<\eta\le1$, then there is $B\subseteq A$ with $|B|\ge c_\eta n$ and both $|B-B|$ and $|B+B|$ bounded by $K_\eta|B|$. The constants depend only on $\eta$. We prove explicit, nonoptimal polynomial bounds, thereby proving the required Balog–Szemerédi statement.

Let $r(s)=|\{(a,a')\in A^2:a+a'=s\}|$. Then $E(A)=\sum_sr(s)^2$. Declare $S=\{s:r(s)\ge\eta n/2\}$ to be the set of [popular sums](../../../../../../popular-sum.md). The remaining sums contribute at most $(\eta n/2)\sum_sr(s)=\eta n^3/2$. Since $r(s)\le n$, it follows that $\sum_{s\in S}r(s)\ge\eta n^2/2$. Also $|S|\le2n/\eta$. Form a [bipartite graph](../../../../../../bipartite-graph.md) on two copies of $A$, joining $a$ to $a'$ when $a+a'\in S$. Its density is at least $\rho=\eta/2$.

We prove the needed [four-step path lemma for a dense bipartite graph](../../../../../../four-step-path-lemma-for-a-dense-bipartite-graph.md). Call an ordered pair of left vertices bad if its number of common right neighbors is less than $\tau n$, where $\tau=\rho^2/32$. For a uniformly chosen right vertex $y$, let $U=N(y)$ and let $b(U)$ count bad ordered pairs in $U^2$. Then

$$
\mathbb E|U|\ge\rho n,\qquad \mathbb Eb(U)\le\tau n^2.
$$

Consequently some $y$ satisfies

$$
|U|-\frac{16b(U)}{\rho n}\ge\frac{\rho n}{2}.
$$

For this $U$, $|U|\ge\rho n/2$ and $b(U)\le\rho n|U|/16\le|U|^2/8$. Delete vertices having more than $|U|/4$ bad partners in $U$. At most half are deleted; the retained set $B$ has $|B|\ge|U|/2\ge\rho n/4$. For any $a,b\in B$, at least $|U|/2$ middle vertices $u\in U$ are good partners of both. Each such $u$ supplies at least $(\tau n)^2$ walks $a,v,u,w,b$ of four edges. Hence every pair in $B$ has at least

$$
\frac{|U|}{2}(\tau n)^2\ge\frac{\rho^5n^3}{4096}
$$

such walks. Repetition of vertices is allowed; it does not affect the counting argument.

Each walk has edge labels

$$
s_1=a+v,\quad s_2=u+v,\quad s_3=u+w,\quad s_4=b+w,
$$

all in $S$, and $a-b=s_1-s_2+s_3-s_4$. For a fixed pair $a,b$, these four labels determine $v,u,w$, so distinct walks have distinct label quadruples. For each element of $B-B$, fix one representing pair $a,b$. Label quadruples for distinct differences cannot overlap. Therefore

$$
|B-B|\frac{\rho^5n^3}{4096}\le|S|^4.
$$

Using $\rho=\eta/2$ and $|S|\le2n/\eta$ yields

$$
\boxed{|B|\ge\frac\eta8n,\qquad |B-B|\le2^{21}\eta^{-9}n
\le2^{24}\eta^{-10}|B|.}
$$

This proves the [small-difference-set form of the Balog-Szemerédi-Gowers theorem](../../../../../../small-difference-set-form-of-the-balog-szemeredi-gowers-theorem.md). To obtain a small sumset too, write $K=2^{24}\eta^{-10}$ and apply the already proved [Plünnecke inequality](../../../../../../plunnecke-inequality.md) to starting set $-B$ and summand set $B$. Some nonempty $X\subseteq-B$ has $|X+2B|\le K^2|X|$. For any fixed $x\in X$, $x+2B\subseteq X+2B$, whence $|B+B|\le K^2|B|$. Thus the conventional small-sumset conclusion also follows with constants depending only on $\eta$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
