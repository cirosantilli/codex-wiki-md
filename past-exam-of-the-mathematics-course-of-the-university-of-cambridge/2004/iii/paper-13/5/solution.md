<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) is a striking example of the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md): an intersection restriction creates a family of [linearly independent](../../../../../linear-independence.md) low-degree [polynomials](../../../../../polynomial-split.md), whose dimension bounds the set family. Let $p$ be a [prime number](../../../../../prime-number.md), let $L\subseteq\mathbb F_p$ have $s$ elements, and let $\mathcal F$ be a [set family](../../../../../set-family.md) such that member sizes modulo $p$ avoid $L$ while every distinct pair has intersection size in $L$ modulo $p$. Its general modular form gives

$$
|\mathcal F|\leq\sum_{j=0}^s\binom nj.
$$

If all members have the same size $k$ and $s\leq k$, the uniform refinement gives **$|\mathcal F|\leq\binom ns$**.

For the proof, work over the [finite field](../../../../../finite-field.md) $\mathbb F_p$ and associate to $A\in\mathcal F$ the [modular intersection polynomial](../../../../../modular-intersection-polynomial.md)

$$
P_A(x)=\prod_{\lambda\in L}\left(\sum_{i\in A}x_i-\lambda\right).
$$

At the [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md) $B$, this equals zero for $B\ne A$ and is nonzero for $B=A$. A linear relation among the evaluation functions therefore has every coefficient zero. The [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md), replacing $x_i^a$ by $x_i$ for $a\geq1$, preserves these evaluations and the degree bound $s$. There are $\sum_{j=0}^s\binom nj$ possible square-free [monomials](../../../../../monomial.md), proving the general form.

For uniform members, the [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md) supplies the sharper dimension bound. To verify this without division modulo $p$, form the integer incidence [matrix](../../../../../matrix.md) with rows indexed by subsets $S$ of size at most $s$, columns indexed by $k$-subsets $B$, and entries $\mathbf1_{S\subseteq B}$. Over the [rational numbers](../../../../../rational-number.md), a row with $|S|=j$ is $\binom{k-j}{s-j}^{-1}$ times the sum of all size-$s$ rows containing $S$. Its [matrix rank](../../../../../matrix-rank.md) is at most $\binom ns$. Every larger integer minor is consequently zero and remains zero modulo $p$, giving the same bound over $\mathbb F_p$. The nonzero diagonal evaluation [matrix](../../../../../matrix.md) of the $P_A$ then forces $|\mathcal F|\leq\binom ns$.

The theorem, proved by Frankl and Wilson in 1981, extends the theme of the [Ray-Chaudhuri–Wilson theorem](../../../../../ray-chaudhuri-wilson-theorem.md) from ordinary intersection sizes to residues. Modular restrictions can be weaker than exact intersection restrictions yet still force unexpectedly small families. Here are three consequences from one explicit [modular intersection graph](../../../../../modular-intersection-graph.md).

Take $N=4p-1$, $k=2p-1$, and let the [vertices](../../../../../vertex-graph-theory.md) be all $k$-subsets of $[N]$, with an [edge](../../../../../edge-of-a-graph.md) exactly when the intersection has size $p-1$. An [independent set](../../../../../independent-set-graph-theory.md) avoids the only possible off-diagonal intersection congruent to $k$ modulo $p$, so applying the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) with $L=\mathbb F_p\setminus\{p-1\}$ gives

$$
\alpha(G)\leq B:=\binom N{p-1}.
$$

A [clique](../../../../../clique-graph-theory.md) has one exact intersection size. Apply the uniform theorem modulo a prime larger than $k$, with $L=\{p-1\}$, to get $\omega(G)\leq N$. Since there are $v=\binom Nk$ [vertices](../../../../../vertex-graph-theory.md), this gives the explicit asymmetric [Ramsey number](../../../../../ramsey-number.md) bound **$R(N+1,B+1)>v$**. It illustrates how algebraic constructions produce graphs with simultaneously restricted [cliques](../../../../../clique-graph-theory.md) and [independent sets](../../../../../independent-set-graph-theory.md).

For a geometric application, map each [vertex](../../../../../vertex-graph-theory.md) to $x_A=\mathbf1_A/\sqrt{2p}$ in $\mathbb R^N$. Then $|x_A-x_B|^2=(k-|A\cap B|)/p$, so [edges](../../../../../edge-of-a-graph.md) have unit [Euclidean distance](../../../../../euclidean-distance.md). Every proper colouring of Euclidean space therefore colours this finite [graph](../../../../../graph-split.md), giving

$$
\chi(\mathbb R^N)\geq\chi(G)\geq\frac{\binom N{2p-1}}{\binom N{p-1}}.
$$

The [Stirling formula](../../../../../stirling-formula.md) gives the ratio as $\exp((\log2-H(1/4)+o(1))N)$, where $H(a)=-a\log a-(1-a)\log(1-a)$ is the [binary entropy function](../../../../../binary-entropy-function.md) in natural-log units. The positive constant $\log2-H(1/4)$ proves an exponential [chromatic number of Euclidean space](../../../../../chromatic-number-of-euclidean-space.md) lower bound along these dimensions.

Finally, a quadratic embedding converts this same forbidden intersection into a forbidden [diameter](../../../../../diameter.md) pair. Set $u_A=2\mathbf1_A-\mathbf1$ and $Q_A=u_Au_A^T$. The [quadratic sign-vector diameter formula](../../../../../quadratic-sign-vector-diameter-formula.md) follows from the [Frobenius inner product](../../../../../frobenius-inner-product.md):

$$
\|Q_A-Q_B\|_F^2=2\bigl(N^2-(u_A\cdot u_B)^2\bigr),
\qquad
u_A\cdot u_B=4|A\cap B|-4p+3.
$$

For distinct members the smallest possible absolute inner product is one, attained exactly when the intersection is $p-1$. Thus maximum-distance pairs are exactly [edges](../../../../../edge-of-a-graph.md) of $G$. The matrices have common diagonal; using their off-diagonal coordinates, multiplied by $\sqrt2$, realizes them isometrically in $D=\binom N2$ dimensions. They are distinct because equal outer products require $u_A=\pm u_B$, and complements have size $2p$, not $k$.

Any subset of smaller [diameter](../../../../../diameter.md) contains at most $B$ points, so a partition into smaller-[diameter](../../../../../diameter.md) pieces needs at least $v/B=\exp(c_0N+o(N))$ pieces. For sufficiently large primes this exceeds $D+1$, disproving the [Borsuk conjecture](../../../../../borsuk-conjecture.md). This is the mechanism behind the [Kahn-Kalai counterexample to the Borsuk conjecture](../../../../../kahn-kalai-counterexample-to-the-borsuk-conjecture.md): the number of required pieces grows exponentially in the original set-system parameter while dimension grows quadratically. Their [1993 paper](https://arxiv.org/abs/math/9307229) establishes the resulting high-dimensional counterexample.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
