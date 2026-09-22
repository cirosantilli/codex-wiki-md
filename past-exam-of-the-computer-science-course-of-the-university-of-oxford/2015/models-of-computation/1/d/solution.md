<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**No: [regular languages](../../../../../regular-language.md) are not closed under countably infinite [intersection](../../../../../set-intersection.md).** Let $\Sigma=\{0,1\}$ and put

$$
K=\{0^n1^n:n\geq0\},\qquad
L_i=\{w\in\Sigma^*:|w|\geq i\}\cup\{0^n1^n:2n<i\},\quad i\geq1.
$$

The first term in $L_i$ has [regular expression](../../../../../regular-expression.md) $(0\cup1)^i(0\cup1)^*$, where the fixed power $i$ means $i$ copies. The second term is a [finite language](../../../../../finite-language.md), a finite [union](../../../../../set-union.md) of single [words](../../../../../string.md). Their [union](../../../../../set-union.md) is therefore a [regular language](../../../../../regular-language.md).

If $w\in K$, then for each $i$ either $|w|\geq i$ or $w$ belongs to the second term, so $w\in L_i$. If $w\notin K$, choose $i>|w|$. It belongs to neither term of $L_i$. Consequently

$$
\boxed{\bigcap_{i=1}^{\infty}L_i=K.}
$$

The [formal language](../../../../../formal-language.md) $K$ is not a [regular language](../../../../../regular-language.md). Indeed, for a proposed [pumping length](../../../../../pumping-length.md) $p\geq1$, the [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md) applied to $0^p1^p$ must pump a nonempty block consisting only of zeros. Repeating that block increases the number of zeros without increasing the number of ones, leaving $K$. This contradiction proves the counterexample. Finite [intersection](../../../../../set-intersection.md) closure does not extend to this [infinite intersection of regular languages](../../../../../infinite-intersection-of-regular-languages.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Models of computation](../../../models-of-computation-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
