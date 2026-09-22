<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No: $R$ cannot contain a nonzero nilpotent element.** We prove the needed principle, [localization detects zero elements](../../../../../../localization-detects-zero-elements.md), rather than assume it.

Let $a\ne0$ in $R$. Its [annihilator](../../../../../../annihilator-ring-theory.md) $\operatorname{Ann}(a)=\{r:ra=0\}$ is a proper [ideal](../../../../../../ideal.md), because $1$ does not annihilate $a$. Every proper [ideal](../../../../../../ideal.md) is contained in a [maximal ideal](../../../../../../maximal-ideal.md), by the [Zorn lemma](../../../../../../zorn-s-lemma.md); choose such a [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$ containing $\operatorname{Ann}(a)$. If $a/1=0$ in $R_{\mathfrak m}$, then some $s\notin\mathfrak m$ satisfies $sa=0$. This would put $s$ in $\operatorname{Ann}(a)\subseteq\mathfrak m$, a contradiction. Thus every nonzero element survives in at least one [localization at a prime ideal](../../../../../../localization-at-a-prime-ideal.md).

Now suppose $a^n=0$. For every [prime ideal](../../../../../../prime-ideal.md) $P$, $(a/1)^n=0$ in $R_P$. The assumed absence of nonzero [nilpotent elements](../../../../../../nilpotent.md) forces $a/1=0$ in every $R_P$. The preceding argument then forces $a=0$. In the terminology of [reduced rings](../../../../../../reduced-ring.md), we have proved

$$
\boxed{R_P\text{ reduced for every prime }P\ \Longrightarrow\ R\text{ reduced}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
