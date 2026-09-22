<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [SMILES string](../../../../../smiles-string.md) encodes a molecular [graph](../../../../../graph-split.md) as a sequence of atom and bond symbols, with parentheses for branches, matching digits for ring closures and additional symbols for charges and [stereochemistry](../../../../../stereochemistry-split.md). For example, 
```
CCO
```
 specifies ethanol. A [molecule](../../../../../molecule-split.md) may have several valid SMILES traversals, so the raw character sequence is not itself a unique physical descriptor.

Two numerical encodings are:

- A [molecular fingerprint](../../../../../molecular-fingerprint.md): a fixed-length vector indicating local substructures, for example hashed circular neighborhoods around atoms. Each coordinate is a bit or a count. The same atom–bond graph should produce the same fingerprint regardless of its SMILES traversal.
- A [molecular descriptor](../../../../../molecular-descriptor.md) vector: real-valued quantities such as [molar mass](../../../../../molar-mass.md), atom counts, formal charge, [hydrogen bond donor](../../../../../hydrogen-bond-donor.md) and [hydrogen bond acceptor](../../../../../hydrogen-bond-acceptor.md) counts, or topological indices. Standardize these coordinates using the training set before fitting a scale-sensitive model.

These are chemical-structure representations. No biological mechanism is needed to encode the [molecules](../../../../../molecule-split.md) or treat the supplied target as a binary label.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
