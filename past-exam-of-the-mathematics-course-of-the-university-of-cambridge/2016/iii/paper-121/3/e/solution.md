<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take the least [omega-measurable cardinal](../../../../../../omega-measurable-cardinal.md) $\kappa$, with a [countably complete ultrafilter](../../../../../../countably-complete-ultrafilter.md) $U$ on $\kappa$ that is nonprincipal. We prove that $U$ is $\kappa$-complete. This will give $\boxed{\kappa\text{ is measurable}}$.

Suppose $\mu<\kappa$, $A_i\in U$ for $i<\mu$, and $\bigcap_{i<\mu}A_i\notin U$. Then $B=\kappa\setminus\bigcap_{i<\mu}A_i$ belongs to $U$. For $x\in B$ let $g(x)$ be the least $i<\mu$ with $x\notin A_i$. The [pushforward ultrafilter](../../../../../../pushforward-ultrafilter.md)

$$
W=\{E\subseteq\mu:g^{-1}[E]\in U\}
$$

is a countably complete [ultrafilter](../../../../../../ultrafilter.md) on $\mu$; this uses $B\in U$, so $U$ restricts to an ultrafilter on $B$. For each $i$, the fibre $g^{-1}[\{i\}]$ is contained in $\kappa\setminus A_i$, hence is not in $U$. Thus $W$ is nonprincipal. If $\mu$ is finite or countable, countable completeness already rules this out. Otherwise $|\mu|<\kappa$ would be an [omega-measurable cardinal](../../../../../../omega-measurable-cardinal.md), contradicting minimality of $\kappa$.

Therefore every intersection of fewer than $\kappa$ members of $U$ lies in $U$. Since $\kappa$ is uncountable, it is a [measurable cardinal](../../../../../../measurable-cardinal.md). This proves that the [least omega-measurable cardinal is measurable](../../../../../../least-omega-measurable-cardinal-is-measurable.md), even if the originally supplied cardinal carried only a countably complete ultrafilter.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
