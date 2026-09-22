<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

A [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) is a tuple $(Q,\Sigma,\delta,q_0,F)$ with finite state set $Q$, finite input alphabet $\Sigma$, transition function $\delta:Q\times\Sigma\to Q$, initial state $q_0$, and accepting-state set $F\subseteq Q$. It accepts a word when the [extended transition function of a deterministic finite automaton](../../../../../extended-transition-function-of-a-deterministic-finite-automaton.md) carries $q_0$ to a state in $F$. A [regular language](../../../../../regular-language.md) is a language accepted by some deterministic finite automaton.

The [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md) says that if a regular language is accepted by an automaton with $N$ states, every accepted word $w$ of length at least $N$ has a decomposition $w=xyz$ with $|xy|\leq N$, $|y|>0$, and $xy^iz$ in the language for every $i\geq0$. Indeed, among the $N+1$ states visited before and after the first $N$ symbols, two are equal by the [pigeonhole principle](../../../../../pigeonhole-principle.md). The intervening nonempty word $y$ labels a loop, which may be traversed any number of times without changing the final accepting state.

In [base two](../../../../../binary-numeral-system.md), the powers of two have representations $10^n$, so their language is the [regular expression](../../../../../regular-expression.md) $10^*$ and is regular.

Suppose instead that their [base-ten representations](../../../../../decimal-representation.md) formed a regular language. Apply the pumping lemma to a sufficiently long decimal power of two $xyz$, and put $d=|y|>0$. Pumping gives decimal integers $a_i$ represented by $xy^iz$, all powers of two. A direct place-value calculation shows that

$$
a_{i+1}-10^d a_i=C
$$

for a constant $C$ independent of $i$. The lengths, and hence the exponents in $a_i=2^{n_i}$, tend to infinity. Dividing by $a_i$ gives

$$
2^{n_{i+1}-n_i}-10^d=\frac C{2^{n_i}}.
$$

For large $i$, the right side has absolute value less than one while the left side is an integer, so it must vanish. This would make a power of two equal to $10^d=2^d5^d$, impossible for $d>0$ by [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md). Thus the decimal powers of two are not a [regular language](../../../../../regular-language.md).

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
