<h1 id="4f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [context-free grammar](../../../../../../context-free-grammar.md) is a quadruple $G=(V,\Sigma,P,S)$ consisting of a finite set $V$ of [nonterminal symbols](../../../../../../nonterminal-symbol.md), a disjoint finite [alphabet](../../../../../../alphabet.md) $\Sigma$ of [terminal symbols](../../../../../../terminal-symbol.md), a start symbol $S\in V$, and a finite set $P$ of [productions](../../../../../../production-rule.md) $A\to\alpha$ with $A\in V$ and $\alpha\in(V\cup\Sigma)^*$. A sentence is a terminal [word over an alphabet](../../../../../../string.md) $w\in\Sigma^*$ with $S\Rightarrow^*w$, and the generated [formal language](../../../../../../formal-language.md) is $\mathcal L(G)=\{w\in\Sigma^*:S\Rightarrow^*w\}$.

The first language is [context-free](../../../../../../context-free-language.md). For example, the productions

$$
S\to aaSbb\mid\varepsilon
$$

generate exactly $\{a^{2m}b^{2m}:m\geq0\}$: each recursive production adds two $a$s to the left and two $b$s to the right.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4F](../../4f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
