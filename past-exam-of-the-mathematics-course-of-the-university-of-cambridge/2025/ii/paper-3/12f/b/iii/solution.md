<h1 id="12f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We induct on the length of $w$. For $w=\varepsilon$, the extended transition set is $\{q\}$, and the sole witnessing sequence is $(q)$, so the claim holds.

Write a nonempty word as $w=va$. By the recursive definition,

$$
q'\in\widehat\Delta(q,va)
$$

if and only if there is some $p\in\widehat\Delta(q,v)$ with $q'\in\Delta(p,a)$. By the induction hypothesis, the first condition on $p$ is equivalent to a witnessing sequence for $v$ from $q$ to $p$. Appending $q'$ gives a witnessing sequence for $va$. Conversely, deleting the last state of any witnessing sequence for $va$ gives just such a state $p$ and sequence for $v$. This proves both implications.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [12F](../../../12f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
