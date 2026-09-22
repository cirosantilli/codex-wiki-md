<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $A$ is finitely generated, the [structure theorem for finitely generated modules over a principal ideal domain](../../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) immediately makes $A/nA$ finite.

Conversely, first replace the given height by a quadratic one. Set

$$
\widehat h(P)=\lim_{r\to\infty}4^{-r}h(2^rP).
$$

Condition (ii) makes this limit converge and gives

$$
|\widehat h(P)-h(P)|\leq\sum_{r\geq0}c_1,4^{-r-1}=\frac{c_1}{3}.
$$

Thus $\widehat h$ still has finite bounded subsets. Condition (i) also gives a global lower bound for $h$, so $\widehat h\geq0$. Applying condition (iii) to $2^rP,2^rQ$, dividing by $4^r$ and passing to the limit gives one direction of the parallelogram identity. Applying the same inequality to $P+Q$ and $P-Q$, and using $\widehat h(2P)=4\widehat h(P)$, gives the reverse direction. Hence

$$
\widehat h(P+Q)+\widehat h(P-Q)
=2\widehat h(P)+2\widehat h(Q),
$$

and induction yields $\widehat h(mP)=m^2\widehat h(P)$ for every integer $m$.

Now suppose $A/nA$ is finite and choose representatives $R_1,\ldots,R_s$. Put $R=\max_i\widehat h(R_i)$. For any $P$, write $P=nQ+R_i$. Nonnegativity and the parallelogram identity give

$$
n^2\widehat h(Q)=\widehat h(P-R_i)
\leq2\widehat h(P)+2\widehat h(R_i),
$$

so, since $n\geq2$,

$$
\widehat h(Q)-R\leq\frac12(\widehat h(P)-R).
$$

Repeated division modulo $nA$ therefore reaches the finite set $B=\{P:\widehat h(P)\leq R+1\}$. Reversing the recursion expresses every element of $A$ using $B$ and the finitely many $R_i$. This is the [height descent lemma](../../../../../../height-descent-lemma.md), and proves

$$
\boxed{A\text{ is finitely generated}\iff|A/nA|<\infty.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
