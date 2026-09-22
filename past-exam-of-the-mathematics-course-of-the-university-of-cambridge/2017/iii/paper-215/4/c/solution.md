<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The reference kernel printed in the hint has total mass $1/n+\binom n2/\binom n2=1+1/n$, so it is not a [Markov kernel](../../../../../../markov-kernel.md). We explicitly replace it by the normalized [random transposition shuffle](../../../../../../random-transposition-shuffle.md): choose two positions independently and uniformly and swap them. Its probabilities are

$$
\widetilde p(\mathrm{id})=1/n,\qquad\widetilde p((i,j))=2/n^2\quad(i<j).
$$

These sum to one, and its ordinary [spectral gap](../../../../../../spectral-gap.md) is $\widetilde\gamma=2/n$, the value intended in the hint. This value can also be certified by the [Aldous spectral gap theorem](../../../../../../aldous-spectral-gap-theorem.md): the single-label generator has rate $2/n^2$ between distinct positions, so on centered functions it acts as multiplication by $-2/n$. Both shuffles have the same [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md) as [stationary distribution](../../../../../../stationary-distribution.md).

We use the [Canonical paths comparison theorem](../../../../../../canonical-paths-comparison-theorem.md) in the following precise form. For two finite [reversible Markov chains](../../../../../../reversible-markov-chain.md) with the same positive [stationary distribution](../../../../../../stationary-distribution.md) $\pi$, route each directed transition $(x,y)$ of $\widetilde P$ along a positive-capacity [path](../../../../../../continuous-path.md) $\eta_{xy}$ of $P$. If

$$
A=\max_{e:Q(e)>0}\frac1{Q(e)}\sum_{x,y}\pi(x)\widetilde P(x,y)|\eta_{xy}|N_e(\eta_{xy}),\qquad Q(u,v)=\pi(u)P(u,v),
$$

then $\widetilde{\mathcal E}(f,f)\leq A\mathcal E(f,f)$ and $\gamma\geq\widetilde\gamma/A$. Indeed, telescope each difference along its [path](../../../../../../continuous-path.md), apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), and sum with weights $\pi(x)\widetilde P(x,y)/2$. The load definition gives the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md) inequality; the common [variance](../../../../../../variance-split.md) denominator then gives the [spectral gap](../../../../../../spectral-gap.md) inequality. Identity transitions use empty [paths](../../../../../../continuous-path.md).

Put $s_k=(k,k+1)$. A [transposition](../../../../../../transposition-permutation.md) $(i,j)$ is routed using the word

$$
s_i s_{i+1}\cdots s_{j-1}s_{j-2}\cdots s_i,
$$

of length $L_{ij}=2(j-i)-1\leq2n$. Each generator occurs at most twice; write its occurrence count as $N_k(i,j)\leq2$. For a fixed directed adjacent edge $(\sigma,\sigma s_k)$ and each occurrence of $s_k$ in a word, there is exactly one starting permutation whose translated word crosses this edge at that occurrence. This follows because right multiplication by the prefix is a [bijection](../../../../../../bijection.md) of the [symmetric group](../../../../../../symmetric-group.md). Hence the uniform stationary factors cancel in the comparison load, leaving

$$
A=\max_k\frac2n\sum_{i<j}L_{ij}N_k(i,j).
$$

The crude bounds $L_{ij}\leq2n$, $N_k(i,j)\leq2$, and $\binom n2\leq n^2/2$ imply $A\leq4n^2$. Therefore

$$
\boxed{\gamma\geq\frac{2/n}{4n^2}=\frac1{2n^3}.}
$$

Only pairs with $i\leq k<j$ contribute, and there are $k(n-k)\leq n^2/4$ of these. Keeping this restriction gives the stronger $A\leq2n^2$ and $\gamma\geq1/n^3$. Neither comparison bound needs the exact adjacent-shuffle [spectral gap](../../../../../../spectral-gap.md); the normalization repair of the reference kernel is essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
