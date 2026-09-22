<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose a uniformly random [permutation](../../../../../permutation.md) of $[n]$ and take its initial segments. This produces a [Uniformly random maximal chain in a Boolean lattice](../../../../../uniformly-random-maximal-chain-in-a-boolean-lattice.md). A fixed $r$-set belongs to this chain with [probability](../../../../../probability.md) $r!(n-r)!/n!=\binom nr^{-1}$. An [antichain](../../../../../antichain.md) meets the chain at most once, so taking the [expected value](../../../../../expected-value.md) of the number of meetings proves the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md):

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\le1.}
$$

In particular the [Sperner theorem](../../../../../sperner-s-theorem.md) bound follows by multiplying each summand by at most the largest [binomial coefficient](../../../../../binomial-coefficient.md).

For the [vector](../../../../../vector.md) request, an ordering by ordinary [subset](../../../../../subset.md) need not work: distinct [vectors](../../../../../vector.md) may cancel. Instead, write $s_A=\sum_{i\in A}x_i$ and construct a [separated block decomposition for vector subset sums](../../../../../separated-block-decomposition-for-vector-subset-sums.md). A block is separated if distinct labeled members have [subset](../../../../../subset.md) sums at distance at least one. We prove that the labeled [subsets](../../../../../subset.md) of $[n]$ can be partitioned into separated blocks, with

$$
b_{n,r}=\binom nr-\binom n{r-1}
$$

blocks of size $n-2r+1$, for $0\le r\le\lfloor n/2\rfloor$, with $\binom n{-1}=0$.

For $n=0$ the one [subset](../../../../../subset.md) forms one block. Suppose a block of sums $z_1,\ldots,z_\ell$ has already been constructed for $n-1$ [vectors](../../../../../vector.md), and let $x=x_n$. Choose $z_*$ minimizing $z_j\cdot x$ in the block. Replace the two copies of the block, with and without the new coordinate, by the following two blocks:

$$
\{z_1+x,\ldots,z_\ell+x,z_*\},\qquad
\{z_j:j\ne *\}.
$$

The old labels are retained, so these partition the two copies even if equal sums occur in different blocks. Translation preserves separation in the first translated portion, and the second block is a [subset](../../../../../subset.md) of the old separated block. For the new cross pairs, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\|z_j+x-z_*\|\ge\frac{(z_j-z_*+x)\cdot x}{\|x\|}
\ge\|x\|\ge1.
$$

Thus both new blocks are separated. Their sizes are $\ell+1$ and $\ell-1$, omitting an empty block. The resulting size-profile recurrence is $b_{n,r}=b_{n-1,r}+b_{n-1,r-1}$, and Pascal's identity verifies the displayed binomial-difference formula, including the even middle boundary. The total number of blocks telescopes to $\binom n{\lfloor n/2\rfloor}$.

A signed sum associated with $A=\{i:\epsilon_i=1\}$ is $2s_A-\sum_i x_i$. If two signed sums lie in the [open ball](../../../../../open-ball.md) of radius one, their difference has [norm](../../../../../norm.md) less than two, so their [subset](../../../../../subset.md) sums have distance less than one. At most one can therefore lie in any separated block. Hence the [Littlewood-Offord inequality](../../../../../littlewood-offord-inequality.md) is

$$
\boxed{\#\left\{\epsilon\in\{-1,1\}^n:\left\|\sum_i\epsilon_ix_i-a\right\|<1\right\}
\le\binom n{\lfloor n/2\rfloor}.}
$$

The counting is by sign choices, not by distinct numerical values of the sums. The open-ball condition handles the equality-distance boundary correctly.

For the last request take real coefficients. Absorb their signs into the choices $\epsilon_i$, so all coefficients are positive and at least one. A signed-sum [real interval](../../../../../interval-mathematics.md) of length four corresponds to a subset-sum [real interval](../../../../../interval-mathematics.md) of length two. A strict three-member inclusion chain $A\subsetneq B\subsetneq C$ would have $s_C-s_A\ge2$, which cannot occur in that open [real interval](../../../../../interval-mathematics.md). Thus its [set family](../../../../../set-family.md) is a [k-Sperner family](../../../../../k-sperner-family.md) with $k=2$. Every [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) meets it at most twice, yielding $\sum_r |\mathcal F_r|/\binom nr\le2$. Write $f_r=|\mathcal F_r|/\binom nr$, so $0\le f_r\le1$ and $\sum_r f_r\le2$. If $B_1\ge B_2$ are the two largest [binomial coefficients](../../../../../binomial-coefficient.md) and $f_*$ is the fraction at a largest level, then $|\mathcal F|\le B_1f_*+B_2(2-f_*)\le B_1+B_2$. This proves the [two-level Littlewood-Offord bound](../../../../../two-level-littlewood-offord-bound.md):

$$
\boxed{\binom n{\lfloor n/2\rfloor}+\binom n{\lfloor(n-1)/2\rfloor}\quad(n\ge1).}
$$

It is the greatest possible number uniformly over choices of coefficients and center. For even $n=2m$, take every coefficient equal to one and center $a=-1$: the [real interval](../../../../../interval-mathematics.md) $(-3,1)$ contains the sum levels $-2,0$, of multiplicities $\binom n{m-1},\binom nm$. For odd $n=2m+1$, take center zero, giving levels $-1,1$, each of multiplicity $\binom nm$. These attain the bound. For $n=0$ the only sign choice gives the separate maximum one. Attainment here is at the exhibited centers; it need not hold at every prescribed center.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
