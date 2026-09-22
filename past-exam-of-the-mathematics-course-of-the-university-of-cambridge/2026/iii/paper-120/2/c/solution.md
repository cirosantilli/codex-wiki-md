<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [crude incompleteness theorem](../../../../../../crude-incompleteness-theorem.md) says that every consistent recursively axiomatized extension $T$ of $PA^-$ is incomplete.

Suppose instead that $T$ were complete. Enumerating proofs until either $\sigma$ or $\neg\sigma$ appears would decide theoremhood, so its characteristic function $\chi_T$ would be total recursive. By the assumed representation theorem, choose a formula $R(x)$ such that $PA^-$ proves $R(\bar n)$ when $\chi_T(n)=1$ and proves $\neg R(\bar n)$ when $\chi_T(n)=0$. The diagonal lemma supplies $\gamma$ with

$$
PA^-\vdash\gamma\leftrightarrow\neg R(\ulcorner\gamma\urcorner).
$$

If $T\vdash\gamma$, then $\chi_T(\ulcorner\gamma\urcorner)=1$, so $T\vdash R(\ulcorner\gamma\urcorner)$ and is inconsistent. If $T\vdash\neg\gamma$, then the characteristic value is zero, so $T\vdash\neg R(\ulcorner\gamma\urcorner)$ and hence $T\vdash\gamma$, again a contradiction. Completeness must therefore fail.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
