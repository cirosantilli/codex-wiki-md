<h1 id="scala-2-11-12-method-type-inference-implementation">Scala 2.11.12 method type inference implementation</h1>

↑ **Parent:** [Computer science bibliography](computer-science-bibliography-split.md)

[https://raw.githubusercontent.com/scala/scala/v2.11.12/src/compiler/scala/tools/nsc/typechecker/Namers.scala](https://raw.githubusercontent.com/scala/scala/v2.11.12/src/compiler/scala/tools/nsc/typechecker/Namers.scala)

The [compiler](compiler.md)'s `methodSig`, `typesFromOverridden`, and `assignTypeToTree` use an inherited return type as an expected type when checking an overriding method body. This permits [numeric widening](numeric-widening.md) of a literal in that body while still inferring more specific reference result types where appropriate.

## ↑ Ancestors (3)

1. [Computer science bibliography](computer-science-bibliography-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/7/c/solution.md)
