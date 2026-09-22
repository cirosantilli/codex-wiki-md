<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

There is a genuine qualification missing from the printed bound. With $n=3,r=1,m=4$, the family of three singletons has distinct intersections of size zero, which is not congruent to $r$ modulo $m$. Nevertheless its size is three, whereas $\binom n{m-1}=\binom33=1$. Thus that bound cannot hold without a restriction on the parameters. The valid [prime-power modular intersection bound](../../../../../prime-power-modular-intersection-bound.md) is

$$
\boxed{|\mathcal F|\leq\binom n{\min(r,m-1)}.}
$$

In particular the printed form holds when $m-1\leq r$.

Put $m=p^a$ with $p$ a [prime number](../../../../../prime-number.md), and $d=m-1$. If $r<d$, the corrected bound is simply the total number $\binom nr$ of $r$-sets. Assume henceforth $d\leq r$. For an integer $z$, consider the residue detector

$$
f(z)=\binom{z-r+d}{d}\pmod p.
$$

For nonnegative upper arguments, the [Lucas theorem](../../../../../lucas-s-theorem.md) and the fact that every base-$p$ digit of $d$ equals $p-1$ show that $f(z)$ is one when $z\equiv r\pmod m$ and zero otherwise. The assertion also holds for negative upper arguments, using integer-valued generalized [binomial coefficients](../../../../../binomial-coefficient.md). Indeed the coefficient of $u^d$ in $(1+u)^q$ is periodic in the integer exponent $q$ modulo $m$: in characteristic $p$, $(1+u)^m=1+u^m$, so multiplying even a [formal power series](../../../../../formal-power-series.md) by $(1+u)^m$ does not change coefficients of degrees below $m$. Reduce any exponent modulo $m$ to obtain the stated detector.

For each $A\in\mathcal F$, apply that detector to $|A\cap B|$. Its evaluations on $B\in\mathcal F$ form the identity matrix, since the diagonal intersection is $r$ and every off-diagonal intersection has a different residue. The detector is represented on Boolean vectors by the [multilinear polynomial](../../../../../multilinear-polynomial.md)

$$
f_A(x)=\sum_{\substack{S\subseteq A\\|S|\leq d}}\binom{d-r}{d-|S|}\prod_{i\in S}x_i\pmod p.
$$

To check this expression, evaluate at the [characteristic vector](../../../../../characteristic-vector-of-a-set.md) of $B$: summing by $j=|S|$ gives $\sum_j\binom{|A\cap B|}j\binom{d-r}{d-j}=\binom{|A\cap B|+d-r}d$ by the coefficient identity for $(1+u)^{|A\cap B|}(1+u)^{d-r}$.

Here is the necessary [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md), with care about characteristic $p$. Let $M$ be the integer incidence [matrix](../../../../../matrix.md) whose rows are subsets $S$ of size at most $d$, whose columns are all $r$-sets $B$, and whose entries are $\mathbf1_{S\subseteq B}$. Over the [rational numbers](../../../../../rational-number.md), for $|S|=j\leq d$ its row satisfies

$$
M_S=\binom{r-j}{d-j}^{-1}\sum_{\substack{T\supseteq S\\|T|=d}}M_T.
$$

Thus its rational [matrix rank](../../../../../matrix-rank.md) is at most $\binom nd$. Every larger square minor has integer determinant zero; reducing those determinants modulo $p$ gives $\operatorname{rank}_{\mathbb F_p}M\leq\binom nd$ too. This argument does not divide by a potentially zero element of the [finite field](../../../../../finite-field.md). The identity evaluation matrix $(f_A(\mathbf1_B))_{A,B\in\mathcal F}$ factors through these incidence rows, so its rank $|\mathcal F|$ is at most $\binom nd$. This proves the qualified bound.

Choose the two-applications alternative. First, the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) yields a constructive lower bound for a [diagonal Ramsey number](../../../../../diagonal-ramsey-number.md). Let $p\geq3$ be prime, set $N=p^3,r=p^2-1$, and use all $r$-subsets of $[N]$ as vertices of a complete graph. Color a pair red when its intersection size is $-1$ modulo $p$, and blue otherwise. A blue [clique](../../../../../clique-graph-theory.md) has size at most $D=\binom N{p-1}$ by the proved bound with modulus $p$. In a red [clique](../../../../../clique-graph-theory.md), all distinct intersections belong to

$$
L=\{p-1,2p-1,\ldots,(p-1)p-1\}.
$$

For each vertex $A$ of that clique, the polynomial $P_A(x)=\prod_{\ell\in L}(\sum_{i\in A}x_i-\ell)$ vanishes at all the other vertices' [characteristic vectors](../../../../../characteristic-vector-of-a-set.md) and is nonzero at its own. Replace repeated powers $x_i^j$ by $x_i$ on Boolean vectors. Its degree is at most $p-1$, so the rational version of the same incidence-rank argument bounds a red [clique](../../../../../clique-graph-theory.md) by $D$ as well. Therefore this two-coloring has neither color containing a clique of size $D+1$, and

$$
\boxed{R(D+1,D+1)>\binom{p^3}{p^2-1},\qquad D=\binom{p^3}{p-1}.}
$$

The usual estimates $(N/k)^k\leq\binom Nk\leq(eN/k)^k$ give $\log D=\Theta(p\log p)$ and $\log\binom{p^3}{p^2-1}=\Theta(p^2\log p)$. Thus along this explicit sequence the [diagonal Ramsey number](../../../../../diagonal-ramsey-number.md) exceeds $\exp(c(\log s)^2/\log\log s)$ for some absolute $c>0$. This is substantially larger than any fixed power of $s$.

Second, obtain an exponential lower bound for the [chromatic number of Euclidean space](../../../../../chromatic-number-of-euclidean-space.md). Let $N=4p-1,r=2p-1$, and join two $r$-subsets exactly when their intersection has size $p-1$. An [independent set](../../../../../independent-set-graph-theory.md) in this graph avoids that intersection. Among the possible distinct intersection sizes $0,\ldots,2p-2$, the only one congruent to $r$ modulo $p$ is $p-1$. Hence every [independent set](../../../../../independent-set-graph-theory.md) has size at most $\binom{4p-1}{p-1}$. Embed each vertex as $v_A=\mathbf1_A/\sqrt{2p}$ in [Euclidean space](../../../../../euclidean-norm.md). Then

$$
\|v_A-v_B\|^2=\frac{2r-2|A\cap B|}{2p},
$$

so the graph's edges have exactly [Euclidean distance](../../../../../euclidean-distance.md) one. Each color class must be an [independent set](../../../../../independent-set-graph-theory.md), giving

$$
\boxed{\chi(\mathbb R^{4p-1})\geq\frac{\binom{4p-1}{2p-1}}{\binom{4p-1}{p-1}}.}
$$

The [Stirling formula](../../../../../stirling-formula.md) makes the logarithm of this ratio $N(\log2-h(1/4))+o(N)$, where $h(x)=-x\log x-(1-x)\log(1-x)$. Since $\log2-h(1/4)>0$, this is an exponential dimensional lower bound for the [chromatic number of Euclidean space](../../../../../chromatic-number-of-euclidean-space.md). Both applications lie in the valid parameter range of the proved modular bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
