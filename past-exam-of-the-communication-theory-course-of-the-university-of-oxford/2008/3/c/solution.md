<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\bar\ell=\mathbb E|c(X)|$. The [Huffman encoder](../../../../huffman-coding.md) emits an average of $w\bar\ell$ binary digits per minute. Shannon's [noisy-channel coding theorem](../../../../noisy-channel-coding-theorem.md) states that for a [discrete memoryless channel](../../../../discrete-memoryless-channel.md) of capacity $K$, every information rate strictly below $K$ bits per use is achievable with error probability tending to zero as block length grows; rates above $K$ are not achievable for unrestricted messages.

Thus a channel code carrying the [Huffman bitstream](../../../../huffman-coding.md) reliably with buffering and arbitrarily long blocks can be chosen whenever

$$
\boxed{rK>w\bar\ell,\qquad r>\frac{w\bar\ell}{K}}.
$$

The strict inequality supplies positive coding and buffering slack. [Huffman's expected-length bound](../../../../huffman-codeword-length-bounds.md) is $H(X)\le\bar\ell<H(X)+1$ for a nontrivial finite source. Therefore the simpler bound $r>w(H(X)+1)/K$ is sufficient without knowing its exact Huffman lengths.

Distinguish this bitstream construction from the absolute source-channel limit. The [noiseless source coding theorem](../../../../shannon-s-source-coding-theorem.md) permits long source blocks to be compressed to any rate above $H(X)$ bits per source symbol, with arbitrarily small overhead. Together with channel coding, this gives the sharper limiting requirement $rK>wH(X)$; $rK<wH(X)$ is impossible by the source-channel converse. Further compression can exploit [redundancy](../../../../redundancy-of-a-binary-prefix-code.md) remaining in a single-symbol Huffman stream, so $w\bar\ell/K$ need not be the universal minimum channel symbol rate. At $K=0$ a positive-[entropy](../../../../information-entropy-split.md) source cannot be sent reliably at a finite rate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
