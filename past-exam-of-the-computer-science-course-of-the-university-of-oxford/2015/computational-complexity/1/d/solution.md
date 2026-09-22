<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**$\mathcal L_{\ell3}$ is [undecidable](../../../../../undecidable-decision-problem.md).** The condition depends only on the accepted [formal language](../../../../../formal-language.md). It holds for a [Turing machine](../../../../../turing-machine.md) accepting the [empty language](../../../../../empty-language.md), and fails for a [Turing machine](../../../../../turing-machine.md) accepting the singleton $\{aaaa\}$, where $a$ is an [alphabet](../../../../../alphabet.md) symbol. It is therefore a nontrivial [extensional property of programs](../../../../../extensional-property-of-programs.md), and [Rice's theorem](../../../../../rice-s-theorem.md) applies. In particular, the condition does not assert that the machine halts on every [input](../../../../../input-computer-science.md); nonacceptance of long [words over an alphabet](../../../../../string.md) may result from rejection or from an infinite computation.

**$\mathcal L_{1\mathrm T}$ is a [decidable language](../../../../../recursive-language.md): it consists of every valid [Turing machine encoding](../../../../../turing-machine-encoding.md).** Every [multitape Turing machine](../../../../../multitape-turing-machine.md) has an equivalent [single-tape Turing machine](../../../../../single-tape-turing-machine.md). To see this, represent the finitely used portions of its tapes on one tape, separated by delimiters, and mark each simulated head position. To simulate one step, scan these portions to read the marked symbols, retain this fixed number of symbols and the control state in finite control, and scan again to update the symbols and head marks. Extend a represented portion with a blank cell when necessary. Each simulated step takes finitely many real steps.

The [single-tape Turing machine](../../../../../single-tape-turing-machine.md) accepts exactly when the simulated [multitape Turing machine](../../../../../multitape-turing-machine.md) accepts; infinite computations remain infinite. The simulation may increase [time complexity](../../../../../time-complexity.md), but the question only asks about accepted [formal languages](../../../../../formal-language.md). Hence a decider simply checks the syntax of the [Turing machine encoding](../../../../../turing-machine-encoding.md) and accepts every valid description. [Rice's theorem](../../../../../rice-s-theorem.md) does not make this property [undecidable](../../../../../undecidable-decision-problem.md), because the property is true of every [computably enumerable language](../../../../../recursively-enumerable-language.md) and is therefore trivial in the theorem's sense.

$$
\boxed{\mathcal L_{\ell3}\text{ is undecidable};\qquad\mathcal L_{1\mathrm T}\text{ is decidable}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
