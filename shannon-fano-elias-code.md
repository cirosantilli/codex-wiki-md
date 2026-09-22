# Shannon-Fano-Elias code

↑ **Parent:** [Prefix code](prefix-code.md)

For positive source [probabilities](probability.md) in a fixed order, let $F_k=\sum_{r<k}p_r$ and $G_k=F_k+p_k/2$. The [Shannon-Fano-Elias code](shannon-fano-elias-code.md) uses the first $l_k$ binary digits of the [midpoint](midpoint.md) $G_k$, using the terminating-zero expansion at [dyadic rationals](dyadic-rational.md). Its [dyadic interval](dyadic-interval.md) contains $G_k$ and has width at most $p_k/2$, so it lies inside the [probability](probability.md) cell $[F_k,F_k+p_k)$. These cells are disjoint, whereas a [codeword](codeword.md) that is a prefix of another has a [dyadic interval](dyadic-interval.md) containing the other [interval](interval-mathematics.md). The code is therefore a [prefix code](prefix-code.md). Since $l_k<-\log_2p_k+2$, averaging proves $\mathbb EL<H(X)+2$. This is a direct cumulative construction and does not require sorting the [probabilities](probability.md) or constructing a Huffman tree.

## ↑ Ancestors (8)

1. [Prefix code](prefix-code.md)
2. [Decipherable code](decipherable-code.md)
3. [Unique decodability](unique-decodability.md)
4. [Coding theory](coding-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2011/2/c/solution.md)
- [Shannon-Fano-Elias code](shannon-fano-elias-code.md)
