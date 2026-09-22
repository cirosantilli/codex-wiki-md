# Double counting (proof technique)

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_counting_(proof_technique))

Double counting establishes an identity by computing the [cardinality](cardinality.md) of the same [finite set](finite-set.md) in two ways. The useful step is to identify exactly what the members of that collection are; an algebraic equality then records two legitimate ways to organize them.

Take the [ordered pairs](ordered-pair.md) $(S,x)$ where $S$ is a $k$-element [subset](subset.md) of an $n$-element [set](set-split.md) and $x\in S$ is marked. Choosing $S$ first gives $k\binom nk$ pairs. Choosing $x$ first leaves $k-1$ members to choose from the other $n-1$, giving $n\binom{n-1}{k-1}$. Hence

$$
k\binom nk=n\binom{n-1}{k-1}\qquad(1\leq k\leq n).
$$

For five people and two-person teams, both counts give $20$: ten teams with two choices of a marked member, or five choices of that member with four choices of a teammate. The identity is explained by the [bijection](bijection.md) between these descriptions, rather than merely verified through [factorials](factorial.md).

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)
