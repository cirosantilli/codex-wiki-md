# Boolean operations on events

↑ **Parent:** [Boolean operation](boolean-operation.md)

[Events](event.md) turn [Boolean operations](boolean-operation.md) into operations on [sets](set-split.md). For a die with [sample space](sample-space.md) $U=\{1,2,3,4,5,6\}$, let $A=\{2,4,6\}$ be the [event](event.md) “even outcome” and $B=\{4,5,6\}$ the [event](event.md) “outcome at least four”. At outcome $u$, use the [indicator functions](indicator-function.md) $P=\mathbf1_A(u)$ and $Q=\mathbf1_B(u)$. Then

$$
\begin{aligned}
\text{AND: }A\cap B&=\{4,6\},&\text{OR: }A\cup B&=\{2,4,5,6\},\\
\text{XOR: }A\mathbin\triangle B&=\{2,5\},&\text{NOT }A:\ U\setminus A&=\{1,3,5\}.
\end{aligned}
$$

Thus [logical conjunction](logical-conjunction.md) becomes [set intersection](set-intersection.md), [logical disjunction](logical-disjunction.md) becomes [set union](set-union.md), [exclusive or](exclusive-or.md) becomes [symmetric difference](symmetric-difference.md), and [logical negation](negation.md) becomes the [complement of a set](complement-of-a-set.md) within $U$. Outcome four satisfies both [events](event.md), so inclusive [logical disjunction](logical-disjunction.md) includes it and [exclusive or](exclusive-or.md) excludes it. If the die is fair, these four [events](event.md) have [probabilities](probability.md) $1/3$, $2/3$, $1/3$, and $1/2$, respectively. No assumption of [independent events](independent-events.md) is needed for the [set](set-split.md) identities; indeed $A$ and $B$ here are not [independent](independent-random-variables.md), since $1/3\ne(1/2)(1/2)$.

## ↑ Ancestors (4)

1. [Boolean operation](boolean-operation.md)
2. [Theoretical computer science](theoretical-computer-science-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [De Morgan's laws](de-morgan-s-laws.md)
- [Negation](negation.md)
