# Information hiding

↑ **Parent:** [Encapsulation (computer programming)](encapsulation-computer-programming.md)

[Information hiding](information-hiding.md) makes an implementation decision the responsibility of one [software module](software-module.md), whose [API](application-programming-interface.md) lets other code work without knowing that decision. For a [FIFO queue](fifo-queue.md), clients need the removal order and failure behavior; they need not know the current front index in an [array](array-data-structure.md). This explains why [encapsulation](encapsulation-computer-programming.md) is useful beyond [object-oriented programming](object-oriented-programming.md): procedures with hidden storage can provide the same boundary.[Parnas, pp. 1054 and 1056, What Is Modularization? and The Criteria: responsibility assignments and hidden design decisions](on-the-criteria-to-be-used-in-decomposing-systems-into-modules-by-d-l-parnas.md)

In [On the Criteria To Be Used in Decomposing Systems into Modules by D. L. Parnas](on-the-criteria-to-be-used-in-decomposing-systems-into-modules-by-d-l-parnas.md) (December 1972, pp. 1054–1056), the example applies a [sorting algorithm](sorting-algorithm.md) to word rotations of [input](input-computer-science.md) lines. One decomposition shares storage layouts among processing stages. The alternative exposes line-storage operations such as `CHAR` and `SETCHAR`, hiding whether characters are packed four to a machine word. Changing that packing then belongs to line storage rather than every client. The paper presents a design argument using a deliberately small example, not a universal measured speedup or a claim that classes are required. It also notes that an unnecessarily specified rotation order restricts future implementations (p. 1056, Improvement in Circular Shift Module).

## ↑ Ancestors (3)

1. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [Information hiding](information-hiding.md)
- [Software module](software-module.md)
