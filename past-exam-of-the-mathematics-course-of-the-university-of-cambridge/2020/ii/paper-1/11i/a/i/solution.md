<h1 id="11i/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [binary block code](../../../../../../../binary-block-code.md) of length $n$ is a subset $C\subseteq\mathbb F_2^n$. Its size is $M=|C|$, and its minimum [Hamming distance](../../../../../../../hamming-distance.md) is

$$
d=\min_{\substack{x,y\in C\\x\ne y}}d_H(x,y).
$$

Thus an $[n,M,d]$ code consists of $M$ binary words of length $n$ whose distinct pairs differ in at least $d$ coordinates. When $d=1$, every set of distinct words qualifies. Taking all of the [binary vector space](../../../../../../../vector-space-over-a-finite-field.md) $\mathbb F_2^n$ gives $2^n$ words, and no code can contain more words than its ambient space. Hence

$$
\boxed{A(n,1)=2^n}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [11I](../../../11i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
