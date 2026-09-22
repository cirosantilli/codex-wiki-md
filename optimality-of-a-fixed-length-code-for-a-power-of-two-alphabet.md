# Optimality of a fixed-length code for a power-of-two alphabet

↑ **Parent:** [Optimal prefix code](optimal-prefix-code.md)

For a strictly positive [probability distribution](probability-distribution-split.md) on $2^n$ source symbols, with $n>1$, every optimal binary [prefix code](prefix-code.md) has common length $n$ if and only if $p_x+p_y>p_z$ for every three distinct symbols. It suffices to compare the sum of the two smallest probabilities with the largest.

An optimal binary prefix tree has no node with only one child, because removing that detour would strictly shorten positive-probability words. It therefore satisfies equality in the [Kraft inequality](kraft-mcmillan-inequality.md). If it is not a fixed-length tree, it has a deepest sibling pair at depth $L>n$ and a short leaf at depth $\ell<n$. Exchanging that pair with the short leaf changes the [expected codeword length](expected-codeword-length.md) by $(L-\ell-1)(p_z-p_x-p_y)$. Strict positivity of every pair sum over a third probability makes this change negative, contradicting optimality.

Conversely, if $p_x+p_y\leq p_z$, begin with the complete depth-$n$ tree, place $x,y$ at sibling leaves, replace their parent by $z$, and replace the previous $z$ leaf by children $x,y$. The new expected length is $n+p_x+p_y-p_z\leq n$ and its lengths are unequal. If the optimum is below $n$, every optimal tree is nonuniform; if it is $n$, this modified tree is a nonuniform optimum. Thus equality in the probability condition already defeats the assertion that every optimum has fixed length.

## ↑ Ancestors (7)

1. [Optimal prefix code](optimal-prefix-code.md)
2. [Huffman coding](huffman-coding.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2009/2/c/solution.md)
