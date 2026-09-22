<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First assume a [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md), as stated above. Let $L$ be the largest [codeword length](../../../../../codeword-length.md) and take a [tree leaf](../../../../../leaf-of-a-tree.md) at depth $L$. Every existing [tree child](../../../../../child-in-a-rooted-tree.md) of its [tree parent](../../../../../parent-in-a-rooted-tree.md) must also be a [tree leaf](../../../../../leaf-of-a-tree.md): an internal [tree child](../../../../../child-in-a-rooted-tree.md) would have a descendant deeper than $L$. If the chosen [tree leaf](../../../../../leaf-of-a-tree.md) were its [tree parent](../../../../../parent-in-a-rooted-tree.md)'s only [tree child](../../../../../child-in-a-rooted-tree.md), moving its symbol to that [tree parent](../../../../../parent-in-a-rooted-tree.md) would shorten its [codeword](../../../../../codeword.md) by one, preserve the [prefix code](../../../../../prefix-code.md) property, and reduce [expected codeword length](../../../../../expected-codeword-length.md) by its positive [probability](../../../../../probability.md). That contradicts optimality. The [tree parent](../../../../../parent-in-a-rooted-tree.md) therefore has at least two [tree children](../../../../../child-in-a-rooted-tree.md), both [tree leaves](../../../../../leaf-of-a-tree.md). A second [codeword](../../../../../codeword.md) has the same first $L-1$ digits and a different last digit, proving the required **deepest [sibling codeword](../../../../../sibling-leaves-in-a-code-tree.md) property** for a [ternary prefix code](../../../../../ternary-prefix-code.md).

For the literal wording allowing zero [probabilities](../../../../../probability.md), take $p=(1,0,0)$ and the [prefix code](../../../../../prefix-code.md) $(0,10,110)$. Its [expected codeword length](../../../../../expected-codeword-length.md) is one, which is minimal: with more than one message an empty [codeword](../../../../../codeword.md) is impossible, so the positive-probability message must have length at least one. Yet the deepest [tree leaf](../../../../../leaf-of-a-tree.md) $110$ has no [sibling codeword](../../../../../sibling-leaves-in-a-code-tree.md). **Thus positivity or an additional convention removing redundant zero-weight branches is needed.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
