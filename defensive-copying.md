# Defensive copying

↑ **Parent:** [Encapsulation (computer programming)](encapsulation-computer-programming.md)

Protect an owned mutable representation by copying mutable data received from clients and by returning independent copies instead of internal mutable objects. Copying only on entry leaves an accessor leak; copying only on exit leaves the constructor argument aliased. For an object containing only primitive fields, a field-by-field copy suffices. Nested mutable references can require a [deep copy](deep-copy.md), immutable components or a stronger ownership contract.

The correctness argument follows aliases: after copying, no client-held reference reaches the owned mutable fields, and every public mutation goes through operations preserving the owner's [representation invariant](representation-invariant.md). Copying is one technique for [encapsulation](encapsulation-computer-programming.md), not a substitute for deciding which state is meant to remain mutable.

## ↑ Ancestors (3)

1. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/7/b/ii/solution.md)
