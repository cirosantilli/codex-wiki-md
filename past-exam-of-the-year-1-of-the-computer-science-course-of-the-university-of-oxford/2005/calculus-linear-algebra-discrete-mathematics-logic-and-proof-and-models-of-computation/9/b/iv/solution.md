<h1 id="9/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $L=\{0^m1^n:m,n\geq0,\ m\ne n\}$, and suppose it were a [regular language](../../../../../../regular-language.md). The [formal language](../../../../../../formal-language.md) $B=0^*1^*$ is a [regular language](../../../../../../regular-language.md). By closure of [regular languages](../../../../../../regular-language.md) under [set difference](../../../../../../set-difference.md),

$$
B\setminus L=\{0^n1^n:n\geq0\}
$$

would be a [regular language](../../../../../../regular-language.md). But the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) rules this out: for pumping length $p$, every permitted pumped block in $0^p1^p$ consists of $k>0$ zeros, and deleting it produces $0^{p-k}1^p$, with unequal counts. This contradiction proves

$$
\boxed{\{0^m1^n:m\ne n\}\text{ is not regular}.}
$$

The closure step can also be realized by a [product automaton](../../../../../../product-automaton.md) accepting when the automaton for $B$ accepts and the automaton for $L$ rejects. If the exponents are instead required to be positive, use $B=0^+1^+$; the same argument applies.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
