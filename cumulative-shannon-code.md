# Cumulative Shannon code

↑ **Parent:** [Shannon coding](shannon-coding.md)

Order source probabilities as $p_1\geq\cdots\geq p_N$, put

$$
b_i=\sum_{j<i}p_j,
\qquad
l_i=\lceil-\log_2p_i\rceil,
$$

and take the first $l_i$ binary digits of $b_i$ as the codeword for symbol $i$. Since $b_j-b_i\geq p_i\geq2^{-l_i}$ for $j>i$, two cumulative probabilities cannot lie in the same dyadic interval selected by the earlier codeword. The resulting code is prefix-free.

**Table of contents**

- [Competitive optimality of the Shannon code](competitive-optimality-of-the-shannon-code.md)

## ↑ Ancestors (9)

1. [Shannon coding](shannon-coding.md)
2. [Prefix code](prefix-code.md)
3. [Decipherable code](decipherable-code.md)
4. [Unique decodability](unique-decodability.md)
5. [Coding theory](coding-theory-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/11k/solution.md)
