<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First construct the [bounded-difference automaton](../../../../../../bounded-difference-automaton.md). Fix $K$ as above, enlarging it if necessary. Its states are the finitely many elements $d\in B_K(1)$, together with a reject state and finite flags recording when padding has started on each tape. The initial state is $1$. Read the pair of words synchronously, padding their ends with a symbol $\#$ representing the identity. If the current prefixes represent $g,h$, the difference state is $d=g^{-1}h$. A letter pair $(u,v)$ updates it by

$$
\boxed{d\longmapsto u^{-1}dv}.
$$

Reject if the new difference lies outside $B_K(1)$; padding must occur only in the final suffix of a tape. The accepting state for the generator $a$ is $d=a$. Induction on the prefix length proves that the machine accepts exactly the padded pairs whose prefix differences stay bounded by $K$ and whose final difference is $a$. In particular it correctly recognizes multiplication by $a$ for any pair of the chosen [combing](../../../../../../combing-of-a-group.md) representatives with adjacent endpoints. Taking accepting state $1$ gives the equality machine.

If the [combing](../../../../../../combing-of-a-group.md) [formal language](../../../../../../formal-language.md) $L$ is regular, take the product with its two word acceptors. These are the usual [group multiplier automata](../../../../../../group-multiplier-automaton.md), accepting exactly $(w_1,w_2)\in L^2$ with $\overline{w_1}^{-1}\overline{w_2}=a$. From a known representative $u\in L$, a [finite-state automaton](../../../../../../finite-state-machine.md) search with its first tape fixed finds a representative $v$ of $\overline u a$: existence is guaranteed, so the breadth-first search terminates. Equality is tested by the identity multiplier. Starting with a representative of $1$, repeat these operations over the generators, identifying equal vertices, to build any prescribed finite-radius region of the [Cayley graph](../../../../../../cayley-graph.md) and all its generator-labelled edges. Iterating multiplication over an input word and testing equality with the identity gives a [word problem](../../../../../../word-problem-for-groups.md) [algorithm](../../../../../../algorithm.md).

A bare geometric [combing](../../../../../../combing-of-a-group.md) does not imply that $L$ is a [regular language](../../../../../../regular-language.md). Nor can a [finite-state automaton](../../../../../../finite-state-machine.md) recognize the indicated endpoint relation on all words without any restriction: in $\mathbb Z=\langle a\rangle$, which has its usual geodesic synchronous [combing](../../../../../../combing-of-a-group.md), fixing the second word to $a$ would make the multiplier for $a$ recognize precisely the first words equal to the identity. Intersecting those words with $a^*(a^{-1})^*$ gives $\{a^n(a^{-1})^n:n\ge0\}$, a nonregular language: pumping the initial block changes its exponent without changing the inverse block, contradicting acceptance of precisely the equal exponents. Thus the literal unrestricted-pair request is false; the machines above recognize bounded fellow-travelling pairs, or full representative-pair relations under the additional automatic-language hypothesis.

Nevertheless the final decidability assertion is true for a synchronous [combable group](../../../../../../combable-group.md), without a regular-language assumption. Here is a terminating filling bound, avoiding any assumption that the given [combing](../../../../../../combing-of-a-group.md) is computable. Let $D$ be the number of words of length at most $K$ over $\Sigma$. A horizontal row of the diagram in part (ii) is encoded by its ordered $n$ rung words, so there are at most $D^n$ possible row types. If two rows have the same word tuple, delete the band between them and identify corresponding labelled rungs. This preserves the outside boundary and leaves a valid diagram of the same short [relators](../../../../../../relator.md). Equivalently, the first column is always at $1$, so identical rung tuples describe the same vertex configuration. Repeatedly remove such bands. At most $D^n$ distinct rows remain, with at most $n$ short-relator cells per layer.

This [finite-state row shortening of a combing diagram](../../../../../../finite-state-row-shortening-of-a-combing-diagram.md) gives the recursive bound $\delta_{R_K}(n)\le n(D^n+1)$. For the given [finite group presentation](../../../../../../finite-group-presentation.md), every short identity in the finite set $R_K$ has some fixed diagram over its defining [relators](../../../../../../relator.md). Let $C$ bound their areas. Replacing each short face by its fixed diagram gives

$$
\boxed{\delta_{\mathcal P}(n)\le Cn(D^n+1)}.
$$

Part 3(ii) now supplies a terminating word decider. This also constructs finite [Cayley graph](../../../../../../cayley-graph.md) regions for a nonregular [combing](../../../../../../combing-of-a-group.md): enumerate words of bounded length, use the decider on $u^{-1}v$ to identify vertices, and use it on $u^{-1}va^{-1}$ to determine the generator edges. The finite ball $B_K(1)$ and transition table of the bounded-difference machines can consequently be computed. The constants depend on a fixed [combing](../../../../../../combing-of-a-group.md) and are not a uniform procedure certifying combability of an arbitrary input [group presentation](../../../../../../group-presentation.md). **Every [finite group presentation](../../../../../../finite-group-presentation.md) of this synchronous combable group has solvable [word problem](../../../../../../word-problem-for-groups.md)**, by the presentation-invariance proof in Q3.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
