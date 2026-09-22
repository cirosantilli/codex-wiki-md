<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For example, take

$$
\boxed{\mathcal L=\{\operatorname{enc}(M):M\text{ has an even number of states}\}.}
$$

This is a [decidable language](../../../../../recursive-language.md): check that the [input](../../../../../input-computer-science.md) is a valid [Turing machine encoding](../../../../../turing-machine-encoding.md), count its declared states, and test the count's [integer parity](../../../../../parity-mathematics.md). There are [Turing machines](../../../../../turing-machine.md) with even state counts and [Turing machines](../../../../../turing-machine.md) with odd state counts, so the [formal language](../../../../../formal-language.md) contains some but not all valid descriptions.

**There is no contradiction with [Rice's theorem](../../../../../rice-s-theorem.md) because this is a syntactic property of the description.** Add one unreachable state to a [Turing machine](../../../../../turing-machine.md), assigning any permitted transitions to it. The accepted [formal language](../../../../../formal-language.md) is unchanged, while the [integer parity](../../../../../parity-mathematics.md) of the state count changes. Thus the property is not an [extensional property of programs](../../../../../extensional-property-of-programs.md), which is an essential hypothesis of [Rice's theorem](../../../../../rice-s-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
