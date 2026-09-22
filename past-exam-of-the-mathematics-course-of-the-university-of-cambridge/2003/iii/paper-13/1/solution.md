<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $m=p^a$, with $p$ a [prime number](../../../../../prime-number.md), and $s=m-1$. The printed bound needs a size qualification: for $n=3$, $k=1$ and $m=4$, all three singletons satisfy the intersection restriction, whereas $\binom3{m-1}=1$. The intended nontrivial [prime-power modular intersection bound](../../../../../prime-power-modular-intersection-bound.md) holds when $s\leq k$; without that qualification the universally valid conclusion is

$$
\boxed{|\mathcal A|\leq\binom n{\min\{k,m-1\}}.}
$$

When $k<s$ this follows simply by counting all $k$-sets. We prove the sharper intended form for $s\leq k$.

Choose an integer $L$ with $Lm>k$ and define the integer-valued [polynomial](../../../../../polynomial-split.md)

$$
P(z)=\binom{z-k+Lm-1}{m-1}.
$$

For $0\leq z\leq k$ its top argument is nonnegative. The bottom argument has all its first $a$ base-$p$ digits equal to $p-1$. The [Lucas theorem](../../../../../lucas-s-theorem.md) therefore gives

$$
P(z)\equiv\begin{cases}1&z\equiv k\pmod m,\\0&z\not\equiv k\pmod m\end{cases}\pmod p.
$$

For every $A\in\mathcal A$, consider $P(\sum_{i\in A}x_i)$ on the [Boolean hypercube](../../../../../boolean-hypercube.md). Its [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md) has degree at most $s$ and integer coefficients: the coefficient of a square-free [monomial](../../../../../monomial.md) is an alternating sum of its integer values on Boolean vertices. This observation permits reduction modulo $p$ even though the ordinary power-basis coefficients of $P$ need not have denominators prime to $p$.

At the [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md) $B\in\mathcal A$, these reduced [polynomials](../../../../../polynomial-split.md) have evaluation matrix equal to the identity modulo $p$. Hence their evaluation functions are [linearly independent](../../../../../linear-independence.md) over $\mathbb F_p$. To count the available functions, let $M$ have rows indexed by subsets $S$ with $|S|\leq s$, columns indexed by all $k$-sets $B$, and entries $\mathbf1_{S\subseteq B}$. Over the [rational numbers](../../../../../rational-number.md), for $|S|=j$,

$$
\mathbf1_{S\subseteq B}=\binom{k-j}{s-j}^{-1}\sum_{\substack{T\supseteq S\\|T|=s}}\mathbf1_{T\subseteq B}.
$$

Thus the [matrix rank](../../../../../matrix-rank.md) over the [rational numbers](../../../../../rational-number.md) is at most $\binom ns$. Every larger integer minor is zero and remains zero modulo $p$, so the same rank bound holds over $\mathbb F_p$. This [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md) proves

$$
\boxed{|\mathcal A|\leq\binom n{m-1}\quad(m-1\leq k).}
$$

For the applications alternative, take a [prime number](../../../../../prime-number.md) $p$, set $N=4p-1$, $k=2p-1$, and let $G$ be the [modular intersection graph](../../../../../modular-intersection-graph.md) on all $k$-subsets of $[N]$, joining distinct sets when their intersection has size $p-1$. An [independent set](../../../../../independent-set-graph-theory.md) avoids the only possible off-diagonal intersection congruent to $k$ modulo $p$, so

$$
\alpha(G)\leq\binom N{p-1},\qquad |V(G)|=\binom Nk.
$$

First embed $A$ as $v_A=\mathbf1_A/\sqrt{2p}$ in [Euclidean space](../../../../../euclidean-norm.md). The [Euclidean distance](../../../../../euclidean-distance.md) satisfies

$$
\|v_A-v_B\|^2=\frac{k-|A\cap B|}{p},
$$

so distance one corresponds exactly to an edge of $G$. Every colour class in a proper [graph colouring](../../../../../graph-coloring.md) is an [independent set](../../../../../independent-set-graph-theory.md), giving the lower bound on the [chromatic number of Euclidean space](../../../../../chromatic-number-of-euclidean-space.md)

$$
\boxed{\chi(\mathbb R^{4p-1})\geq\left\lceil\frac{\binom{4p-1}{2p-1}}{\binom{4p-1}{p-1}}\right\rceil.}
$$

The [Stirling formula](../../../../../stirling-formula.md) gives $\log_2\binom N{\lfloor qN\rfloor}=NH(q)+O(\log N)$, where $H$ is the [binary entropy function](../../../../../binary-entropy-function.md). Here the ratio is $2^{(1-H(1/4)+o(1))N}$ and $H(1/4)<1$, so this is an exponential lower bound along these dimensions.

Second set $u_A=2\mathbf1_A-\mathbf1$ and represent $A$ by the off-diagonal entries $\sqrt2\,u_{A,i}u_{A,j}$, $i<j$, of the [symmetric matrix](../../../../../symmetric-matrix.md) $u_Au_A^T$. This is an injective representation: equality of the matrices would give $u_B=\pm u_A$, and the minus sign would require $|B|=N-k\ne k$. The common diagonal can be omitted without changing distances. The [Frobenius inner product](../../../../../frobenius-inner-product.md) gives the [quadratic sign-vector diameter formula](../../../../../quadratic-sign-vector-diameter-formula.md)

$$
\|u_Au_A^T-u_Bu_B^T\|_F^2=2\bigl(N^2-(4|A\cap B|-4p+3)^2\bigr).
$$

The term inside the square is congruent to $3$ modulo $4$, and its smallest possible absolute value is one, attained exactly at $|A\cap B|=p-1$. Such pairs exist. Consequently the diameter pairs of this finite set in dimension $D=\binom N2$ are precisely the edges of $G$. Every part of strictly smaller [diameter](../../../../../diameter.md) is an [independent set](../../../../../independent-set-graph-theory.md) and has at most $\binom N{p-1}$ points. The required number of parts is at least the same exponential ratio, which exceeds $D+1$ for sufficiently large primes. Thus **bounded sets need not admit a partition into $D+1$ sets of smaller diameter**: this supplies a [Kahn-Kalai counterexample to the Borsuk conjecture](../../../../../kahn-kalai-counterexample-to-the-borsuk-conjecture.md). Both applications use the prime case of the proved prime-power result.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
