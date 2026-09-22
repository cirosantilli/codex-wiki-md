<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

These [strings](../../../../../../string.md) are the even-length [palindromes](../../../../../../palindrome.md) $uu^R$. Suppose this were a [regular language](../../../../../../regular-language.md), and let $p$ be its length from the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md). The [string](../../../../../../string.md)

$$
w=0^p110^p
$$

belongs to the [formal language](../../../../../../formal-language.md), with $u=0^p1$. In any allowed decomposition $w=abc$, where $|ab|\leq p$ and $|b|>0$, the pumped block is $b=0^k$ with $1\leq k\leq p$. Pumping it away gives

$$
ac=0^{p-k}110^p.
$$

This is not a [palindrome](../../../../../../palindrome.md): its initial and final runs of zeros have different lengths. Hence it cannot have the form $uu^R$, contradicting the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md). Therefore

$$
\boxed{\{uu^R:u\in\{0,1\}^*\}\text{ is not regular}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2005](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
