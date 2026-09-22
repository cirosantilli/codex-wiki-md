<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $n>0$; the empty case is immediate. Write $r(s)=\#\{(a,b)\in A^2:a-b=s\}$. The [additive energy](../../../../../../additive-energy.md) in the hypothesis is $\sum_sr(s)^2$: rearranging $x+y=z+w$ gives $x-z=w-y$. Since $r(s)\leq n$, the energy is at most $n^3$, so the substantive range is $0<\alpha\leq1$.

Let $S=\{s:r(s)\geq\alpha n/2\}$. The contribution of the other differences to the energy is at most $(\alpha n/2)\sum_sr(s)=\alpha n^3/2$. Consequently

$$
\sum_{s\in S}r(s)^2\geq\alpha n^3/2,\quad\sum_{s\in S}r(s)\geq\alpha n^2/2,\quad |S|\leq2n/\alpha.
$$

Make a [bipartite graph](../../../../../../bipartite-graph.md) with two copies of $A$, joining a left vertex $a$ to a right vertex $b$ when $a-b\in S$. Put $\rho=\alpha/2$. This [graph](../../../../../../graph-split.md) has at least $\rho n^2$ edges, and $|S|\leq n/\rho$.

We prove the needed dense-graph selection rather than quote the [Balog-Szemerédi-Gowers theorem](../../../../../../balog-szemeredi-gowers-theorem.md). A pair of left vertices is bad if it has fewer than $\tau n$ common right neighbours, where $\tau=\rho^2/32$. Choose a right vertex $y$ uniformly, let $U=N(y)$, and let $b(U)$ be the number of ordered bad pairs in $U$. Averaging the degrees gives $\mathbb E|U|\geq\rho n$. Every bad pair lies in fewer than $\tau n$ of these neighbourhoods, so $\mathbb Eb(U)\leq\tau n^2$. Therefore some $y$ satisfies

$$
|U|-\frac{16b(U)}{\rho n}\geq\rho n-\frac{16\tau n}{\rho}=\rho n/2.
$$

For this neighbourhood, $|U|\geq\rho n/2$ and $b(U)\leq\rho n|U|/16\leq|U|^2/8$. Delete vertices having more than $|U|/4$ bad partners in $U$. At most half are deleted, so the remaining [set](../../../../../../set-split.md) $B$ has $|B|\geq|U|/2\geq\rho n/4$.

For any $b,b'\in B$, at least $|U|/2$ vertices $v\in U$ are good partners of both. Each such $v$ has at least $\tau n$ common neighbours with $b$ and at least $\tau n$ with $b'$. Independently choosing those neighbours gives at least

$$
\frac{|U|}{2}(\tau n)^2\geq\frac{\rho^5n^3}{4096}
$$

four-edge walks $b,u,v,w,b'$. Repeated vertices cause no difficulty. This proves the [four-step path lemma for a dense bipartite graph](../../../../../../four-step-path-lemma-for-a-dense-bipartite-graph.md) in the required form.

The labels of such a walk are $s_1=b-u$, $s_2=v-u$, $s_3=v-w$, $s_4=b'-w$, all in $S$, and

$$
b-b'=s_1-s_2+s_3-s_4.
$$

For a fixed pair $(b,b')$, its label tuple uniquely recovers $u=b-s_1$, $v=u+s_2$, and $w=v-s_3$, so distinct walks have distinct label tuples. Choose one pair representing each element of the [difference set](../../../../../../difference-set.md) $B-B$. Tuples belonging to different differences are disjoint because their alternating sum determines that difference. Hence

$$
|B-B|\frac{\rho^5n^3}{4096}\leq|S|^4\leq n^4\rho^{-4}.
$$

We have obtained explicit constants for the [small-difference-set form of the Balog-Szemerédi-Gowers theorem](../../../../../../small-difference-set-form-of-the-balog-szemeredi-gowers-theorem.md):

$$
\boxed{|B|\geq\frac\alpha8n,\qquad |B-B|\leq4096\left(\frac2\alpha\right)^9n.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
