<h1 id="10/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [context-free grammar](../../../../../../context-free-grammar.md) with start symbol $P$, terminal [alphabet](../../../../../../alphabet.md) $\{0,1\}$, and the following productions generates all binary [palindromes](../../../../../../palindrome.md):

$$
\boxed{P\longrightarrow\epsilon\mid0\mid1\mid0P0\mid1P1.}
$$

Each production preserves the [palindrome](../../../../../../palindrome.md) property: it either supplies a central [string](../../../../../../string.md) of length zero or one, or wraps the same symbol around a shorter [palindrome](../../../../../../palindrome.md). This proves soundness by [structural induction](../../../../../../structural-induction.md) on the [parse tree](../../../../../../parse-tree.md).

Conversely, any [palindrome](../../../../../../palindrome.md) of length at least two has equal first and last symbols. Remove them to obtain a shorter [palindrome](../../../../../../palindrome.md), apply [mathematical induction](../../../../../../mathematical-induction.md) on length, and then use the corresponding wrapping production. The three base cases are $\epsilon$, $0$, and $1$, proving completeness.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
