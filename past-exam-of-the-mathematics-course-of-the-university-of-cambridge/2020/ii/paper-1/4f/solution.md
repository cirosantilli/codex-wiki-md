<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

An [alphabet](../../../../../alphabet.md) $\Sigma$ is a finite nonempty set of symbols. A [word over an alphabet](../../../../../string.md) is a finite sequence of symbols from $\Sigma$, including the empty word $\epsilon$; the set of all words is $\Sigma^*$. A [formal language](../../../../../formal-language.md) over $\Sigma$ is any subset $L\subseteq\Sigma^*$.

A [regular expression](../../../../../regular-expression.md) is defined recursively from $\varnothing$, $\epsilon$, and the individual symbols $a\in\Sigma$ by the operations of finite union, concatenation, and [Kleene star](../../../../../kleene-star.md). Its language is defined by

$$
L(\varnothing)=\varnothing,\qquad
L(\epsilon)=\{\epsilon\},\qquad
L(a)=\{a\},
$$



$$
L(R\mid S)=L(R)\cup L(S),\qquad
L(RS)=L(R)L(S),\qquad
L(R^*)=L(R)^*.
$$

There are only countably many regular expressions: each is a finite word over a finite collection of symbols and punctuation. On the other hand, for every nonempty finite alphabet, $\Sigma^*$ is countably infinite, so its [power set](../../../../../power-set.md) $\mathcal P(\Sigma^*)$ is uncountable by the [Cantor theorem](../../../../../cantor-s-theorem.md). Thus there are uncountably many languages but only countably many languages denoted by regular expressions. Consequently

$$
\boxed{\text{some languages over }\Sigma\text{ are not regular}}.
$$

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
