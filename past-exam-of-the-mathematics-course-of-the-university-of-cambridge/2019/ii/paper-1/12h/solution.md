<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Let $\widehat\delta$ be the [extended transition function of a deterministic finite automaton](../../../../../extended-transition-function-of-a-deterministic-finite-automaton.md). States $p,q\in Q$ are equivalent, or indistinguishable, when

$$
p\sim q
\iff
\bigl(\widehat\delta(p,w)\in F
\Longleftrightarrow
\widehat\delta(q,w)\in F\bigr)
\quad\text{for every }w\in\Sigma^*.
$$

The [quotient deterministic finite automaton by indistinguishable states](../../../../../quotient-deterministic-finite-automaton-by-indistinguishable-states.md) $D/{\sim}$ has state set $Q/{\sim}$, initial state $[q_0]$, accepting states $\{[q]:q\in F\}$, and transition

$$
\overline\delta([q],a)=[\delta(q,a)].
$$

Right invariance of $\sim$ makes this well-defined, and the quotient accepts $L(D)$.

To prove minimality, choose for each state $q$ of the accessible automaton $D$ a word $w_q$ with $\widehat\delta_D(q_0,w_q)=q$. Run the same word in any DFA $A$ accepting $L(D)$, and assign the class $[q]$ the reached state of $A$. If two distinct classes $[p]\ne[q]$ reached the same state of $A$, every continuation $u$ would have the same acceptance result after $w_p$ and $w_q$. Since $A$ and $D$ accept the same language, this would make $p$ and $q$ indistinguishable in $D$, a contradiction. Thus $A$ has at least one distinct state for every class in $D/{\sim}$, proving that the quotient is the [minimal deterministic finite automaton](../../../../../minimal-deterministic-finite-automaton.md).

For divisibility by seven, take states $Q=\{0,1,\ldots,6\}$, initial state $0$, accepting set $F=\{0\}$, and transitions

$$
\boxed{\delta(r,b)=2r+b\pmod7},
\qquad b\in\{0,1\}.
$$

After reading a word, the state is its binary value modulo seven, so this [binary divisibility automaton](../../../../../binary-divisibility-automaton.md) accepts exactly the multiples of seven, with leading zeros allowed. Every state is accessible: the three-bit words representing $0,1,\ldots,6$ reach the corresponding residues.

For distinct residues $p,q$, let $w_p$ be the three-bit representation of $-p\pmod7$, chosen in $\{0,\ldots,6\}$. Since $2^3\equiv1\pmod7$, reading $w_p$ from state $p$ ends at

$$
2^3p+(-p)=0\pmod7,
$$

whereas reading it from $q$ ends at $q-p\ne0$. Thus $w_p$ distinguishes $p$ from $q$. All seven states are pairwise distinguishable, so the DFA is minimal by the [Myhill-Nerode theorem](../../../../../myhill-nerode-theorem.md).

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
