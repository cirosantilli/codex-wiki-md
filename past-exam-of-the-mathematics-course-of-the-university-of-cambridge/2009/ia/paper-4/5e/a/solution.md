<h1 id="5e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [left inverse](../../../../../../left-inverse.md) of $f$ is a function $\ell:B\to A$ satisfying $\ell\circ f=\operatorname{id}_A$. If such $\ell$ exists and $f(a)=f(a')$, applying $\ell$ gives $a=a'$, so $f$ is an [injection](../../../../../../injective-function.md). Conversely, suppose $f$ is an [injection](../../../../../../injective-function.md) and fix $a_0\in A$, possible because $A$ is nonempty. Define

$$
\ell(b)=\begin{cases}a,&b=f(a)\text{ for some }a\in A,\\a_0,&b\notin f(A).\end{cases}
$$

The first value is unique by injectivity, and $\ell(f(a))=a$ for every $a$. Thus

$$
\boxed{f\text{ is injective}\iff f\text{ has a left inverse}.}
$$

No choice from a family of nonempty sets is needed here: each preimage in the first case is unique, and the second case uses one fixed element.

A [right inverse](../../../../../../right-inverse.md) is a function $r:B\to A$ with $f\circ r=\operatorname{id}_B$. Its existence makes every $b$ the image of $r(b)$, proving that $f$ is a [surjection](../../../../../../surjective-function.md). Conversely, if $f$ is a [surjection](../../../../../../surjective-function.md), every [fiber of a function](../../../../../../fiber-of-a-function.md) $f^{-1}(\{b\})$ is nonempty. Using the usual [axiom of choice](../../../../../../axiom-of-choice.md) for arbitrary sets, choose $r(b)\in f^{-1}(\{b\})$ for each $b$. Then $f(r(b))=b$, giving

$$
\boxed{f\text{ is surjective}\iff f\text{ has a right inverse}\quad\text{assuming choice}.}
$$

The converse in this second equivalence is the [right-inverse characterization of the axiom of choice](../../../../../../right-inverse-characterization-of-the-axiom-of-choice.md); it is not an unrestricted choice-free theorem about arbitrary sets.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
