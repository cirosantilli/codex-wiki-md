# Redundancy of a binary prefix code

↑ **Parent:** [Prefix code](prefix-code.md)

The redundancy of a binary [prefix code](prefix-code.md) is its [expected codeword length](expected-codeword-length.md) minus the [Shannon entropy](information-entropy-split.md) of its source. It measures the excess number of binary digits per source symbol above the information lower bound. For a full [prefix tree of a code](prefix-tree-of-a-code.md), let $s_v$ be the probability of visiting an interior node $v$ and let $t_v$ be the conditional probability of taking its zero branch. Then

$$
\bar\ell=\sum_v s_v,\qquad H(X)=\sum_vs_vh(t_v),\qquad R=\sum_vs_v[1-h(t_v)],
$$

where $h$ is [binary entropy](binary-entropy.md). The first identity counts one digit for each visited interior node. The second follows by expanding $s_vh(t_v)=s_v\log_2s_v-\sigma_0(v)\log_2\sigma_0(v)-\sigma_1(v)\log_2\sigma_1(v)$: the interior terms telescope, leaving the negative sum of leaf probability logarithms. The final identity follows by subtraction. It makes nonnegativity immediate and proves that zero redundancy occurs exactly when each positive-mass branch decision is balanced. Consequently the leaf probabilities then equal $2^{-\ell_x}$.

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

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2008/3/c/solution.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2008/4/b/solution.md)
