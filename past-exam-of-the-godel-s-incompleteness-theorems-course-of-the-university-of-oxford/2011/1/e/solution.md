<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $T=S+\{\operatorname{Con}_S\}$ and assume $T$ is consistent. The allowed arithmetizations of the previous equivalences give

$$
S\vdash\neg B(\neg R)\leftrightarrow\operatorname{Con}_S,\qquad S\vdash\neg B(\neg G)\leftrightarrow\operatorname{Con}(T).
$$

Suppose $S\vdash R\to G$. Its contrapositive is $\neg G\to\neg R$, and the [Hilbert-Bernays-Löb derivability conditions](../../../../hilbert-bernays-lob-derivability-conditions.md) then give

$$
S\vdash B(\neg G)\to B(\neg R),\qquad S\vdash\neg B(\neg R)\to\neg B(\neg G).
$$

Combining with the two internal equivalences yields $S\vdash\operatorname{Con}_S\to\operatorname{Con}(T)$. Since $T$ contains $\operatorname{Con}_S$, it would prove $\operatorname{Con}(T)$, contrary to the given [Gödel second incompleteness theorem](../../../../godel-second-incompleteness-theorem.md) for this consistent extension. Hence

$$
\boxed{S\nvdash R\to G\quad\text{if }S+\{\operatorname{Con}_S\}\text{ is consistent}.}
$$

Together with the preceding implication, this is the [Strict Gödel-to-Rosser implication](../../../../strict-godel-to-rosser-implication.md) under the stated consistency hypothesis.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
