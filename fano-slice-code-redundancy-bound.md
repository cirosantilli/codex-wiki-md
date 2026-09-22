# Fano slice code redundancy bound

↑ **Parent:** [Shannon-Fano coding](shannon-fano-coding.md)

Recursively split an ordered list of positive source probabilities into contiguous blocks, choosing each cut to minimize the difference between the total masses of the two children. The resulting binary [prefix code](prefix-code.md) has [expected codeword length](expected-codeword-length.md) less than $H+2$, where $H$ is its source [Shannon entropy](information-entropy-split.md). If the probabilities were in nonincreasing order, its expected length is less than $H+1$.

To prove this, an interior node of mass $S$ with child masses $A,B$ contributes $S$ to the expected path length and $S h(A/S)$ to the [Shannon entropy](information-entropy-split.md), by the [chain rule for information entropy](chain-rule-for-information-entropy.md). The inequality $1-h(t)\le|2t-1|$ bounds that node's redundancy by $|A-B|$. If the cut is between probabilities $p_k,p_{k+1}$, shifting the cut by one position cannot improve the imbalance. On the heavier side this gives $|A-B|\le p_k$ or $p_{k+1}$, respectively; a singleton heavier side gives the same inequality directly. Thus $|A-B|\le\max(p_k,p_{k+1})$.

Every original inter-symbol gap is used once in the recursive tree. Summing over gaps bounds total redundancy by $\sum_{k=1}^{m-1}(p_k+p_{k+1})=2-p_1-p_m<2$. In sorted order it is instead at most $\sum_{k=1}^{m-1}p_k=1-p_m<1$. These are expected-length guarantees, not an assertion that the resulting code is always optimal.

## ↑ Ancestors (9)

1. [Shannon-Fano coding](shannon-fano-coding.md)
2. [Prefix code](prefix-code.md)
3. [Decipherable code](decipherable-code.md)
4. [Unique decodability](unique-decodability.md)
5. [Coding theory](coding-theory-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2007/2/c/solution.md)
