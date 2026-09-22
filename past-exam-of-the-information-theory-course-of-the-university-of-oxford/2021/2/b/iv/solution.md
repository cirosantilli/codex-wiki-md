<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

With a [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md), suppose two distinct [tree parents](../../../../../parent-in-a-rooted-tree.md) at depth $L-1$ each have exactly two [tree children](../../../../../child-in-a-rooted-tree.md), both [tree leaves](../../../../../leaf-of-a-tree.md). Move one [tree leaf](../../../../../leaf-of-a-tree.md) from the second pair into the vacant third [tree child](../../../../../child-in-a-rooted-tree.md) slot of the first [tree parent](../../../../../parent-in-a-rooted-tree.md). Its length remains $L$, so this relocation does not change [expected codeword length](../../../../../expected-codeword-length.md). The second [tree parent](../../../../../parent-in-a-rooted-tree.md) now has a single [tree child](../../../../../child-in-a-rooted-tree.md), which is a [tree leaf](../../../../../leaf-of-a-tree.md). Replace that remaining [tree child](../../../../../child-in-a-rooted-tree.md)'s [codeword](../../../../../codeword.md) by the [tree parent](../../../../../parent-in-a-rooted-tree.md)'s word. This preserves the [prefix code](../../../../../prefix-code.md) property and shortens a positive-probability [codeword](../../../../../codeword.md) by one. [Expected codeword length](../../../../../expected-codeword-length.md) strictly decreases, a contradiction. Thus **there is at most one deepest pair with exactly two [sibling codewords](../../../../../sibling-leaves-in-a-code-tree.md)**.

If zero-probability symbols are retained without a reduction convention, the claim can fail. The [probability mass function](../../../../../probability-mass-function.md) $(1,0,0,0,0)$ with [prefix code](../../../../../prefix-code.md) $(0,100,101,110,111)$ has the optimal [expected codeword length](../../../../../expected-codeword-length.md) one, yet contains the two deepest pairs $(100,101)$ and $(110,111)$. The contraction would only shorten a zero-probability word.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
