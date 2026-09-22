# Entropy rate and coding length

↑ **Parent:** [Entropy rate](entropy-rate.md)

Consider a [binary Markov source](binary-markov-source.md) with fair initial [bit](bit.md) and flip [probability](probability.md) $q=1/8$. Its exact $n$-symbol [information entropy](information-entropy-split.md) is $H_n=1+(n-1)h_2(1/8)$. At $n=16$,

$$
H_{16}\simeq9.15346665\ \text{bits},\qquad H_{16}/16\simeq0.57209167\ \text{bits per symbol}.
$$

This includes the uncertainty of the initial [bit](bit.md); the [entropy rate](entropy-rate.md) itself is $h_2(1/8)\simeq0.54356444$ [bits](bit.md) per symbol. The finite-block difference is $(1-h_2(1/8))/n$.

For any finite block distribution, the [entropy lower bound for prefix codes](entropy-lower-bound-for-prefix-codes.md) gives [expected codeword length](expected-codeword-length.md) $L_n\geq H_n$, while [Shannon coding](shannon-coding.md) achieves $L_n<H_n+1$. These bounds apply to each block as one source symbol, without requiring consecutive blocks to be independent. Here [Huffman coding](huffman-coding.md) on all $2^{16}$ possible 16-symbol words gives the independently calculated value $L_{16}\simeq9.19511361$ [bits](bit.md) per block, or $0.57469460$ [bits](bit.md) per symbol. The noninteger value is an [expected value](expected-value-split.md); each actual [codeword](codeword.md) has an integer length. As the block length grows, the [prefix code](prefix-code.md) bounds squeeze $L_n/n$ towards the [entropy rate](entropy-rate.md) when an optimal code is used.

<a id="image-fair-marginal-bits-can-have-a-lower-entropy-rate-with-a-finite-block-initial-cost"></a>
![](entropy-rate-block-cost-and-flip-probability.png)

**[Figure 25](#image-fair-marginal-bits-can-have-a-lower-entropy-rate-with-a-finite-block-initial-cost). Fair marginal bits can have a lower entropy rate, with a finite-block initial cost**. The left panel shows the exact [binary entropy](binary-entropy.md) $h_2(q)$ for the symmetric [binary Markov source](binary-markov-source.md); each individual symbol still has one [bit](bit.md) of [information entropy](information-entropy-split.md). Both near-persistence $q\approx0$ and near-alternation $q\approx1$ make the next symbol predictable. The right panel uses $q=1/8$ and plots $H_n/n=h_2(q)+(1-h_2(q))/n$, rather than literal fractional [codeword lengths](codeword-length.md). The [Huffman coding](huffman-coding.md) point is the exact expected length over all 16-symbol words.

An [entropy rate](entropy-rate.md) below one does not allow every word to fit into a shorter fixed binary word with zero error. For $0<q<1$, all $2^n$ binary words are possible, so an injective fixed-length code needs at least $n$ [bits](bit.md). Compression instead exploits variable [codeword lengths](codeword-length.md), or the vanishing-error convention in [reliable source encoding at a rate](reliable-source-encoding-at-a-rate.md). These are different guarantees.

## ↑ Ancestors (6)

1. [Entropy rate](entropy-rate.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
