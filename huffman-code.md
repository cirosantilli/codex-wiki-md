# Huffman code

↑ **Parent:** [Huffman coding](huffman-coding.md)

A Huffman code is the [prefix code](prefix-code.md) returned by [Huffman coding](huffman-coding.md); the [algorithm](algorithm-split.md) chooses a [code tree](prefix-tree-of-a-code.md), while the code specifies the actual symbol-to-[codeword](codeword.md) assignment. For the [probability distribution](probability-distribution-split.md) $(0.4,0.3,0.2,0.1)$ in symbol order $A,B,C,D$, the illustrated [binary tree](binary-tree.md) gives

$$
c(A)=0,\qquad c(B)=10,\qquad c(C)=110,\qquad c(D)=111.
$$

The [codeword lengths](codeword-length.md) are $1,2,3,3$. This is a [prefix code](prefix-code.md) because no complete [codeword](codeword.md) is an initial segment of another complete [codeword](codeword.md). Thus a decoder can start at the [root of a tree](root-of-a-tree.md), follow one [edge](edge-of-a-graph.md) per [bit](bit.md), emit a symbol on reaching its leaf, then restart at the [root of a tree](root-of-a-tree.md). In particular, `011010111` splits as `0 | 110 | 10 | 111` and decodes to $A,C,B,D$. No separators are transmitted: the leaf tells the decoder where a [codeword](codeword.md) ends.

The [expected codeword length](expected-codeword-length.md) is

$$
L(c)=\sum_xp_x\,|c(x)|=0.4\cdot1+0.3\cdot2+0.2\cdot3+0.1\cdot3=1.9
$$

[bits](bit.md) per source symbol. Four symbols would require $2$ [bits](bit.md) each if all [codewords](codeword.md) had the same length, so this [Huffman code](huffman-code.md) saves $0.1$ [bit](bit.md) per symbol on average, or $5\%$ of that fixed-length payload. A particular message can grow: $A,C,B,D$ uses nine [bits](bit.md) here instead of eight. These lengths count the encoded symbols only; transmitting a code description or message framing can add further cost.

The [Kraft inequality](kraft-mcmillan-inequality.md) is saturated by this [Huffman code](huffman-code.md):

$$
2^{-1}+2^{-2}+2^{-3}+2^{-3}=1.
$$

Its [Shannon entropy](information-entropy-split.md) is

$$
H(X)=-\sum_xp_x\log_2p_x\approx1.846439
$$

[bits](bit.md) per symbol, slightly below the [expected codeword length](expected-codeword-length.md) $1.9$. The [entropy lower bound for prefix codes](entropy-lower-bound-for-prefix-codes.md) applies to every binary [prefix code](prefix-code.md) for this [probability distribution](probability-distribution-split.md). It need not be attainable with integer [codeword lengths](codeword-length.md) for individual symbols; [Huffman coding](huffman-coding.md) reaches the best mean within that class. [David J. C. MacKay, Information Theory, Inference, and Learning Algorithms, chapter 5, section 5.4: symbol-code bounds](https://web.iitd.ac.in/~sumeet/mackay.pdf)

<a id="image-probability-weighted-codeword-lengths-sum-to-1-9-bits-per-symbol-between-entropy-and-fixed-length"></a>
![](huffman-code-length-and-entropy.png)

**[Figure 22](#image-probability-weighted-codeword-lengths-sum-to-1-9-bits-per-symbol-between-entropy-and-fixed-length). Probability-weighted codeword lengths sum to 1.9 bits per symbol, between entropy and fixed length**.

A [Huffman code](huffman-code.md) need not be unique. In the first example, the tied $B$ and $CD$ weights can exchange their $0/1$ [edge](edge-of-a-graph.md) labels, changing [codewords](codeword.md) but preserving their [codeword lengths](codeword-length.md). Ties can also change the lengths themselves. For a second [probability distribution](probability-distribution-split.md) $(0.4,0.2,0.2,0.2)$, first merge $C,D$ to weight $0.4$. The next merge can join $B$ with either $A$ or the $CD$ [subtree](subtree.md), since both have weight $0.4$. Joining $B$ with $A$ permits $A\mapsto00,B\mapsto01,C\mapsto10,D\mapsto11$, with all lengths $2$. Joining $B$ with the $CD$ [subtree](subtree.md) permits $A\mapsto0,B\mapsto10,C\mapsto110,D\mapsto111$, with lengths $1,2,3,3$. Both are [optimal prefix codes](optimal-prefix-code.md) with [expected codeword length](expected-codeword-length.md) $2$: for the latter, $0.4\cdot1+0.2\cdot2+0.2\cdot3+0.2\cdot3=2$. Tie choices can change the [code tree](prefix-tree-of-a-code.md) without changing the minimum mean.

// Target: algebra.bigb

**Table of contents**

- [Uniform-source Huffman length distribution](uniform-source-huffman-length-distribution.md)

## ↑ Ancestors (6)

1. [Huffman coding](huffman-coding.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Binary tree](binary-tree.md)
- [Deflate block framing](deflate-block-framing.md)
- [Deflate Huffman coding](deflate-huffman-coding.md)
- [Deflate overlapping copy](deflate-overlapping-copy.md)
- [Full binary tree](full-binary-tree.md)
- [Huffman code](huffman-code.md)
- [Huffman coding](huffman-coding.md)
- [Optimal prefix code](optimal-prefix-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/d/solution.md)
- [Uniform-source Huffman length distribution](uniform-source-huffman-length-distribution.md)
