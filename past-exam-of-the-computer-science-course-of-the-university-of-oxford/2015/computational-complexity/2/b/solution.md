<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [linear speedup theorem](../../../../../linear-speedup-theorem.md) concerns [multitape Turing machines](../../../../../multitape-turing-machine.md) whose finite control and tape [alphabet](../../../../../alphabet.md) may change. Formally, for $k>1$, if a deterministic $k$-tape [Turing machine](../../../../../turing-machine.md) decides $A$ within $T(n)$ steps on every [input](../../../../../input-computer-science.md) of length $n$, then for every constant $c>0$ there is a deterministic $k$-tape [Turing machine](../../../../../turing-machine.md) deciding the same [formal language](../../../../../formal-language.md) with

$$
\boxed{T_c(n)\leq\frac{T(n)}c+n+O(1).}
$$

The additive constant is independent of $n$; in the usual normalized formulation the bound is $T(n)/c+n+2$, with the integer-rounding convention absorbed in the constant.[Slides 47–48, PDF pp. 62–63: statement for k \> 1 and block simulation](../../../../../computational-complexity-slides-1-by-paul-w-goldberg-2023.md)

The construction packs a fixed number of old tape symbols into each new symbol and uses a larger finite control to simulate blocks of old steps. Initial [input](../../../../../input-computer-science.md) packing explains the additive linear term. If $T(n)/n\to\infty$, choosing a larger constant $c$ makes the total asymptotic [time complexity](../../../../../time-complexity.md) an arbitrarily small constant multiple of $T(n)$.

**It does not promise arbitrary speed increases on fixed hardware.** Larger packed symbols and transition tables cease to be single constant-cost hardware operations without limit. The theorem also retains the [input](../../../../../input-computer-science.md)-reading overhead. It is a statement about changing the abstract machine description and primitive operations, rather than an unlimited implementation optimization on one processor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
