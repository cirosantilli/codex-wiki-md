<h1 id="4j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume that $L$ is context-free and let $p$ be its pumping length. Apply the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md) to

$$
w=a^pb^pa^p.
$$

Write $w=uvxyz$, with $|vxy|\leq p$ and $|vy|>0$. The substring $vxy$ meets at most two of the three constant-letter blocks.

If $v$ and $y$ affect only the first block, only the middle block, or only the last block, pumping down immediately makes the final block length differ from the minimum of the first two lengths. If they meet the first and second blocks, pumping down decreases at least one of those block lengths while leaving the final length $p$, again violating the defining minimum.

It remains that they meet the second and third blocks. Let pumping change their lengths by $s$ and $t$, respectively. Pumping down fails unless $s=t$. If $s=t>0$, pumping up gives lengths

$$
p,\qquad p+s,\qquad p+s,
$$

whose last entry is not $\min(p,p+s)=p$. Thus some pumping exponent always leaves $L$, contradicting the lemma. Hence

$$
\boxed{L\text{ is not context-free}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4J](../../4j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
